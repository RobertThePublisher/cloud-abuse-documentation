# manifesto ya matumizi mabaya ya wingu

Uchanganuzi wa kiufundi wa kutumia GitHub kama kiendeshi cha hifadhi ya kibinafsi kisicho na kikomo cha Terabyte 1, kwa nini miundombinu ya biashara inaiashiria kama ulaghai, na udanganyifu halisi wa kuamini faili zako muhimu za kibinafsi kwenye jukwaa la kudhibiti chanzo.

---

## ⚡ Hesabu ya Matumizi Mabaya

GitHub imeundwa kwa ajili ya ufuatiliaji wa msimbo unaotegemea maandishi, si kwa ajili ya kuhifadhi maudhui ghafi. Kuweka Terabyte 1 ya data katika hazina tofauti zaidi ya 1,000 husababisha arifa za mfumo otomatiki karibu mara moja.

* **Usanidi:** hazina 1,000, kila moja ikiwa na mipaka ya juu ya ukubwa wa faili (kawaida 50MB–100MB kwa kila faili ili kuepuka kizuizi kigumu cha Git).
* **Vekta:** Kutumia mfumo wa hifadhi ya blob wa Git kama safu ya Hifadhi Iliyounganishwa ya Mtandao (NAS) isiyo na kikomo, iliyotengwa.

* **Ukweli:** Hati otomatiki za kupambana na ulaghai hufuatilia kasi ya uundaji wa hazina, alama ya akaunti yote, na miundo ya jozi isiyo ya msimbo (kama `.mp4`, `.zip`, `.iso`).

---

## 🚨 Kwa Nini Imetiwa Alama kama Ulaghai

Sheria na Masharti ya Huduma ya GitHub (ToS) yanakataza waziwazi kutumia upangishaji wa hazina kwa hifadhi ya jumla ya wingu. Hivi ndivyo miundombinu inavyogundua na kuashiria usanidi huu:

| Kipimo cha Kichocheo | Kizingiti kimefikiwa | Kitendo cha Mfumo |
| :--- | :--- | :--- | :--- |
| **Hesabu ya Marejeo** | Hifadhi zaidi ya 1,000 zinazotumika | Akaunti imetiwa alamisho kwa ajili ya ukaguzi wa kufuata sheria kwa mikono. |
| **Alama ya Data** | ~Jumla ya Terabyte 1 | Arifa ya kasi ya hifadhi imesababishwa. |
| **Saini za Faili** | Uwiano mkubwa wa matone ya jozi dhidi ya maandishi | Imetiwa alamisho kiotomatiki kama matumizi mabaya ya miundombinu isiyo ya msimbo. |

---

## 🛑 Udanganyifu wa "Wingu la Kibinafsi"

Kufikiri GitHub ni hifadhi salama na ya kudumu kwa faili zako za faragha ni udanganyifu mkubwa wa usalama na uhifadhi wa data.

### 1. Kufutwa kwa Akaunti ya Notisi Isiyo na Taarifa
Wakati hati otomatiki ya kuzuia ulaghai inapogundua 1TB ya matone ya binary yaliyoenea kwenye mabaki elfu ya taka, akaunti yako haipati barua ya onyo. Inapata **marufuku kali**. Tokeni zako za ufikiaji hufutwa mara moja, na 1TB yako ya data hutoweka kwenye utupu.

### 2. Git Sio Mfumo wa Faili
Git hufuatilia faili kwa kutumia grafu ya acyclic iliyoelekezwa (DAG) ya vitu vya commit. Inahamisha kila kitu. Kusukuma faili kubwa ambazo haziwezi kukusanywa kwenye Git hufanya ufuatiliaji wa historia ya eneo lako kuwa mzito sana, polepole, na unaoweza kuharibika wakati wa mizunguko mikubwa ya kusukuma.

### 3. Faragha Kabisa Hakuna Faragha
Isipokuwa unalipia viwango vya juu vya biashara, kuweka kiasi kikubwa cha data katika hazina za umma huweka faili zako za kibinafsi kwenye vichakataji vya kimataifa, injini za utafutaji, na vihifadhi vya hifadhi otomatiki. Hata kama repo ni ya faragha, mifumo ya GitHub huchanganua maudhui ili kutekeleza sheria za usalama wa jukwaa.

---

## ⚠️ Urejeshaji wa Dharura (Kabla ya Marufuku)

Ikiwa akaunti yako inaonekana hivi hivi sasa, data yako iko kwenye usaidizi wa maisha. Iondoe mara moja.

```bash
# 1. Lazimisha kurejesha data yako muhimu kwenye mashine ya ndani
git clone [https://github.com/username/critical-backup-repo.git](https://github.com/username/critical-backup-repo.git)

# 2. Toa faili ghafi kutoka kwa mfumo wa ufuatiliaji wa Git
mv critical-backup-repo/my-files/ /path/to/local/external/hard-drive/

# 3. Ondoa hazina ya mbali ili kupunguza wasifu wa akaunti yako
# (Fanya hivi kupitia API ya GitHub au paneli ya mipangilio ya hazina mwenyewe)
