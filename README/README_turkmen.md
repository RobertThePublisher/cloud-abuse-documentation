# bulut-abuse-manifest

GitHub-y 1 Terabaýt çäksiz şahsy saklama diski hökmünde ulanmagyň tehniki düşündirişi, kärhana infrastrukturasynyň näme üçin ony galplyk hökmünde belleýändigi we möhüm şahsy faýllaryňyzy çeşme gözegçilik platformasyna ynanmagyň arassa aldawçylygy.

---

## ⚡ Gizlinligiň matematikasy

GitHub çig media arhiwlemek üçin däl-de, tekst esasynda kod yzarlamak üçin niýetlenendir. 1000+ aýry-aýry boş ammarlara 1 Terabaýt maglumat geçirmek awtomatlaşdyrylan ulgam duýduryşlaryny derrew işe girizýär.

* **Gurnama:** 1000 ammar, her biri faýl ölçeginiň iň ýokary çäkleri bilen doldurylan (adatça Git blokunyň öňüni almak üçin her faýl üçin 50MB–100MB).
* **Wektor:** Git-iň blob saklama ulgamyny mugt, merkezleşdirilmedik Network Attached Storage (NAS) gatlagy hökmünde ulanmak.
* **Hakykat:** Awtomatlaşdyrylan galplyga garşy skriptler repozitoriýanyň döredilmeginiň tizligini, hasaplaryň umumy yzyny we kod däl ikilik gurluşlaryny (meselem, `.mp4`, `.zip`, `.iso`) gözegçilik edýär.

---

## 🚨 Näme üçin galplyk hökmünde bellenilýär

GitHub-yň Hyzmat Şertleri (ToS) umumy bulut saklama üçin repozitoriýa hostingini ulanmagy açyk gadagan edýär. Infrastrukturanyň bu gurluşy nähili anyklaýandygyny we belleýändigini takyk görkezýär:

| Tetikleýji metrik | Bosaga ýetildi | Ulgamyň Hereketi |
| :--- | :--- | :--- |
| **Repo Sany** | 1000+ işjeň repozitoriýa | Hasap el bilen laýyklyk gözden geçirilmesi üçin bellendi. |
| **Maglumat yzlary** | ~1 Terabaýt jemlenen | Saklama tizliginiň anomaliýa duýduryşy işe girizildi. |
| **Faýl Gollary** | Ikilik bloblaryň tekste garşy ýokary gatnaşygy | Kod däl infrastrukturanyň nädogry ulanylmagy hökmünde awtomatiki bellendi. |

---

## 🛑 "Şahsy bulut" aldawlary

GitHub-yň şahsy faýllaryňyz üçin howpsuz, hemişelik bunkerdigini pikir etmek uly howpsuzlyk we maglumatlary saklamak illýuziýadyr.

### 1. Nol duýduryşsyz hasap pozulmagy
Awtomatlaşdyrylan galplyga garşy skript müň sany gereksiz ammarda ýaýran 1TB ikilik bloblary anyklanda, hasabyňyza duýduryş haty gelmeýär. Ol **berk gadaganlyk** alýar. Giriş belgileriňiz derrew ýatyrylýar we 1TB maglumatyňyz boşluga ýitip gidýär.

### 2. Git faýl ulgamy däl
Git faýllary commit obýektleriniň gönükdirilen asiklik grafiki (DAG) arkaly yzarlaýar. Ol ähli zady heş edýär. Git-e kompilýasiýa edilmeýän uly faýllary goýmak ýerli taryhy yzarlamagy örän agyr, haýal we uly push aýlawlarynda zaýalanmaga meýilli edýär.

### 3. Mutlak Nol Gizlinlik
Eger siz premium kärhana derejeleri üçin töleg tölemeýän bolsaňyz, köp mukdarda maglumatlary umumy ammarlarda saklamak şahsy faýllaryňyzy global skreperlere, gözleg motorlaryna we awtomatlaşdyrylan ammar arhiwleýjilerine açýar. Hatda ammar hususy bolsa-da, GitHub ulgamlary platforma howpsuzlyk düzgünlerini berjaý etmek üçin mazmuny skanirleýär.

---

## ⚠️ Gyssagly ýagdaýda dikeltmek (gadagan edilmezinden öň)

Eger hasabyňyz häzir şeýle görünýän bolsa, maglumatyňyz durmuş goldawy ulgamynda. Ony derrew öçüriň.

```bash
# 1. Esasy maglumatlaryňyzy ýerli maşyna mejbury gaýtaryň
git klony [https://github.com/username/critical-backup-repo.git](https://github.com/username/critical-backup-repo.git)

# 2. Çig faýllary Git yzarlaýyş ulgamyndan çykaryň
mv critical-backup-repo/my-files/ /path/to/local/external/hard-drive/

# 3. Hasap profiliňizi peseltmek üçin uzakdaky ammary arassalaň
# (Muny GitHub API ýa-da ammar sazlamalary paneli arkaly el bilen ediň)
