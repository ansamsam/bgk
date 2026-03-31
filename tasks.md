# pusulam MVP - Uygulama Görev Listesi

## 1) Temel Altyapı
- [ ] Next.js + Tailwind mobil-first iskeletini kur ve yayın için hazırla.
- [ ] Ortak renk paletini tanımla (yesil, mavi, soft pembe, kahverengi).
- [ ] PWA icin sonraki adimlari planla (`next-pwa`, offline cache stratejisi).

## 2) Auth ve Profil
- [ ] Supabase Auth ile E-posta/Sifre giris-kayit akisini kur.
- [ ] Giris sonrasi `Profil/Dashboard` gorunumunu ac.
- [ ] Profilde `Cozdugum Sorular`, `Basari Oranim`, `Kritik 20 Ilerlemem` kartlarini goster.

## 3) Dinamik Ders ve Is Sektoru
- [ ] Kullaniciya sinif (1-12) ve is sektoru secimi sun.
- [ ] Sinif + derse gore heatmap (Kirmizi: kritik, Sari: oneri, Yesil: tekrar) olustur.
- [ ] Ana ekrana `10 Dakikalik Hizli Ders` secici ekle.

## 4) Gemini Entegrasyonu
- [ ] Gemini API route kur (`/api/gemini`) ve sektor bazli anlatim uret.
- [ ] Ders detayinda `Sektorel Anlatim` sekmesini calistir.
- [ ] `Kaldirac-Araba Krikosu` benzeri is odakli benzetmelerle icerik karti dondur.

## 5) Kritik 20 Simulasyonu
- [ ] MEB AOL gecmis soru tiplerini temsil eden mock veri yapisi kur.
- [ ] `Kritik 20` butonu ile 20 soruluk test baslat.
- [ ] Coktan secmeli cevaplama ve basari/ilerleme guncellemesini bagla.

## 6) Mentor Akisi
- [ ] Ust bolume `Aktif Mentorler` bandi ekle.
- [ ] Her ders ozetinin altina buyuk `Anlamadim, Mentore Soru Gonder` butonu koy.
- [ ] Buton ile acilan modalda goruntu yukleme, not ve gonderim aksiyonunu tamamla.
- [ ] Basarili gonderimde kullaniciya onay mesaji goster.
- [ ] `Mentorlerim` bolumu icin `online/offline` durumlarini listele.

## 7) Navigasyon ve Kullanim
- [ ] Alt/yan menude `Dashboard`, `Derslerim`, `Mentorlerim`, `Ayarlar` sekmelerini ekle.
- [ ] Yuksek kontrastli, buyuk butonlu dark mode arayuzu tum ekranlarda koru.
- [ ] 15 dakikalik odaklanma icin kisa kart akisina gecis butonu ekle.

## 8) Supabase Veri Modeli (MVP)
- [ ] `mentors` tablosu: `id`, `name`, `expertise`, `status`.
- [ ] `questions` tablosu: `student_id`, `mentor_id`, `image_url`, `status`.
- [ ] Soru iletiminde gerekli satirlari `pending` olarak olustur.

## 9) Yayina Hazirlik
- [ ] Vercel ortam degiskenlerini (`SUPABASE`, `GEMINI`) guvenli sekilde tanimla.
- [ ] Hata izleme icin Sentry entegrasyonunu sonraki sprintte ekle.
- [ ] CI/CD (GitHub Actions) ile lint/build dogrulamasini otomatiklestir.
