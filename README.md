# macbooksat

Bu repo, **tek sayfalık bir landing page** içerir. Amaç, kullanıcıyı WhatsApp üzerinden iletişime geçirip MacBook satışı için hızlı ön teklif sürecini başlatmaktır.

## Proje yapısı

- `index.html.txt`: Sayfanın tüm HTML + CSS içeriğini tek dosyada barındırır.
  - `<head>` bölümünde SEO başlık/açıklama meta alanları vardır.
  - `<style>` içinde bileşen sınıfları tanımlanır (`.container`, `.badge`, `.highlights`, `.cta-box`, `.whatsapp-btn` vb.).
  - `<body>` içinde içerik blokları sırasıyla badge, başlık, açıklama, avantaj pill’leri, CTA alanı ve footer olarak yer alır.

## Önemli noktalar

1. **WhatsApp linki özelleştirilmeli**
   - `href="https://wa.me/905XXXXXXXXX?..."` alanı gerçek numara ile değiştirilmelidir.
2. **Dosya uzantısı**
   - İçerik HTML olsa da dosya adı `index.html.txt`. Yayına alırken `index.html` adıyla servis edilmesi gerekir.
3. **Tasarım tamamen inline CSS ile yönetiliyor**
   - Harici CSS/JS yok; değişiklikler doğrudan bu dosya üzerinden yapılır.
4. **Mobil odaklı ve minimal responsive yaklaşım**
   - Temel düzen mobil-first; yalnızca başlık boyutu için bir `@media (min-width: 640px)` kuralı bulunur.

## Yeni başlayan biri için öğrenme sırası

1. `index.html.txt` içinde HTML iskeletini oku.
2. CSS sınıflarının hangi bloklara bağlandığını takip et.
3. CTA akışını incele (`<a class="whatsapp-btn">`).
4. SEO metinlerini ve satış dilini (başlık, alt metin, footer) güncelleme pratiği yap.
5. Dosyayı `index.html` olarak çalıştırıp tarayıcıda görünümü doğrula.

## Sonraki aşamada önerilen geliştirmeler

- İçeriği bileşenleştirmek (ör. ayrı CSS dosyası).
- Basit analitik ölçümü eklemek (CTA tıklama takibi).
- Farklı kampanya sürümleri için A/B varyantları hazırlamak.
- Telefon numarası ve mesaj metnini env/config yaklaşımıyla yönetmek.
