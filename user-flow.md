Bu doküman, bir Açık Öğretim Lisesi (AÖL) öğrencisinin platformdaki yolculuğunu ve sistemin arka planda nasıl çalıştığını özetler.

1. Giriş ve Onboarding (Karşılama)
Başlangıç: Kullanıcı pusulam-mvp.vercel.app adresine gelir.

Giriş/Kayıt: * E-posta ve şifre ile giriş yapar (Veya bypass moduyla doğrudan geçer).

Sektör Seçimi: Kullanıcı çalışmak istediği alanı seçer (Sanayi, Tekstil, Satış, Tarım, Lojistik).

Sınıf Seçimi: Öğrenci güncel sınıfını seçer (1-12. sınıf arası).

2. Dinamik Dashboard (Ana Panel)
Ders Listesi: Seçilen sınıfa göre dersler (Matematik, Fizik, Kimya vb.) otomatik yüklenir.

Odak Modu: Kullanıcı 15 dakikalık "Kritik Odak" sayacını başlatabilir.

İlerleme Takibi: Çözülen soru sayısı ve başarı oranı profil özetinde görünür.

3. Sektörel Anlatım Döngüsü (Gemini AI)
Ders Seçimi: Kullanıcı bir ders kartına tıklar (Örn: Fizik).

AI İstek: Sistem arka planda lib/gemini.ts üzerinden şu verileri Gemini 1.5 Flash'a gönderir:

Sınıf + Ders + Kullanıcının Sektörü

Anlatım: Gemini, konuyu kullanıcının iş hayatından örneklerle (Örn: Sanayi krikosu ile kaldıraçlar) 4 maddede açıklar.

Görsel Destek: Konuyla ilgili profesyonel kaynaklara (YouTube, EBA) yönlendirme butonları aktifleşir.

4. Kritik 20 - Sınav ve Geri Bildirim
Soru Çözümü: Kullanıcı MEB/AÖL tarzı çoktan seçmeli soruları cevaplar.

Anlık Kontrol: * Doğru: Şık yeşil yanar, kısa açıklama görünür.

Yanlış: Şık kırmızı yanar, doğru şık işaretlenir ve "Neden yanlış?" açıklaması çıkar.

Hata Analizi: Yanlış yapılan sorular otomatik olarak "Takıldığım Sorular" listesine kaydedilir.

5. Profil ve Başarım
Başarılarım: Kullanıcının hangi derslerde daha iyi olduğunu gösteren grafikler.

Takıldığım Sorular: Yanlış yapılan soruların tekrar çözülebileceği özel alan.

Ayarlar: Sektör veya sınıf değişikliği yapıldığında tüm içerik anında güncellenir.
