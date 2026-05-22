# bulut-kötüye-kullanımı-manifestosu

GitHub'ı 1 Terabaytlık sonsuz kişisel depolama sürücüsü olarak kullanmanın teknik bir analizi, kurumsal altyapının bunu neden sahtekarlık olarak işaretlediği ve kritik kişisel dosyalarınızı bir kaynak kontrol platformuna emanet etmenin saf bir yanılgı olduğu.

---

## ⚡ Kötüye Kullanımının Matematiği

GitHub, ham medya arşivleme için değil, metin tabanlı kod izleme için tasarlanmıştır. 1.000'den fazla ayrı sahte depoya 1 Terabayt veri yüklemek, neredeyse anında otomatik sistem uyarılarını tetikler.

* **Kurulum:** Her biri maksimum dosya boyutu sınırlarıyla (Git'in sert engellemesini önlemek için genellikle dosya başına 50MB-100MB) dolu 1.000 depo.

* **Vektör:** Git'in blob depolama sistemini ücretsiz, merkezi olmayan bir Ağ Bağlantılı Depolama (NAS) katmanı olarak kullanmak.

* **Gerçeklik:** Otomatik dolandırıcılık önleme komut dosyaları, depo oluşturma hızını, toplam hesap ayak izini ve kod dışı ikili yapıları (örneğin `.mp4`, `.zip`, `.iso`) izler.

---

## 🚨 Neden Dolandırıcılık Olarak İşaretleniyor?

GitHub'ın Hizmet Şartları (ToS), depo barındırmayı genel bulut depolama için kullanmayı açıkça yasaklamaktadır. İşte altyapının bu kurulumu nasıl algıladığı ve işaretlediği:

| Tetikleyici Ölçüt | Eşik aşıldı | Sistem Eylemi |

| :--- | :--- | :--- |

| **Depo Sayısı** | 1.000+'den fazla aktif depo | Hesap manuel uyumluluk incelemesi için işaretlendi. |

| **Veri Ayak İzi** | ~1 Terabayt kümülatif | Depolama hızı anormalliği uyarısı tetiklendi. |

| **Dosya İmzaları** | İkili blob'ların metne oranı yüksek | Kod dışı altyapı suistimali olarak otomatik olarak işaretlendi. |

---

## 🛑 "Kişisel Bulut" Yanılgısı

GitHub'ın özel dosyalarınız için güvenli, kalıcı bir sığınak olduğunu düşünmek, büyük bir güvenlik ve veri saklama yanılgısıdır.

### 1. Sıfır Bildirimli Hesap Silme
Otomatik dolandırıcılık önleme betiği, binlerce gereksiz depoya yayılmış 1 TB'lık ikili veri bloğunu tespit ettiğinde, hesabınıza bir uyarı mektubu gönderilmez. **Kesin bir yasaklama** uygulanır. Erişim belirteçleriniz anında iptal edilir ve 1 TB'lık veriniz yok olur.

### 2. Git Bir Dosya Sistemi Değildir
Git, dosyaları taahhüt nesnelerinin yönlendirilmiş döngüsel olmayan bir grafiği (DAG) kullanarak izler. Her şeyi hash'ler. Büyük, derlenemeyen dosyaları Git'e itmek, yerel geçmişi izlemeyi son derece ağır, yavaş ve büyük push döngüleri sırasında bozulmaya yatkın hale getirir.

### 3. Mutlak Sıfır Gizlilik
Premium kurumsal katmanlar için ödeme yapmadığınız sürece, büyük miktarda veriyi herkese açık depolarda tutmak, kişisel dosyalarınızı küresel veri toplayıcılarına, arama motorlarına ve otomatik depo arşivleyicilerine maruz bırakır. Depo özel olsa bile, GitHub sistemleri platform güvenlik kurallarını uygulamak için içeriği tarar.

---

## ⚠️ Acil Kurtarma (Yasaklanmadan Önce)

Hesabınız şu anda böyle görünüyorsa, verileriniz yaşam desteğinde demektir. Hemen kurtarın.

```bash
# 1. Önemli verilerinizi yerel makinenize zorla geri çekin
git clone [https://github.com/username/critical-backup-repo.git](https://github.com/username/critical-backup-repo.git)

# 2. Ham dosyaları Git izleme sisteminden çıkarın
mv critical-backup-repo/my-files/ /path/to/local/external/hard-drive/

# 3. Hesabınızın profilini düşürmek için uzak depoyu temizleyin
# (Bunu GitHub API'si veya depo ayarları paneli aracılığıyla manuel olarak yapın)
