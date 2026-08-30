# hub

Kişisel projelerimin giriş sayfası. mugiatama34.github.io kökünde yayınlanıyor.

## Amaç
Telefondan tek kısayolla açtığım, projelerime link veren statik sayfa.
Başka hiçbir işlevi yok.

## Kesin kısıtlar
- Tek dosya: index.html. CSS ve JS aynı dosyanın içinde.
- Build adımı yok, paket yok, framework yok.
- Dış kaynak yok: CDN, harici font, analytics, izleme scripti kullanma.
  Sistem fontları yeterli.
- JS sadece gerçekten gerekiyorsa. Sade linkler için gerekmiyor.

## Tasarım
- Mobil öncelikli. Tasarımı dar ekrandan başlat, geniş ekrana genişlet.
- Dark mode varsayılan; prefers-color-scheme ile light varyant.
- Renkler, boşluklar ve yazı boyutları CSS değişkeni olarak tanımlanmalı.
  Bu değişkenler başka bir repoda (stock-analysis) tekrar kullanılacak.
- Dokunma hedefleri en az 44px.

## İçerik yapısı
Her proje bir kart: başlık, tek satır açıklama, link.
Mevcut kartlar:
- stock-paper-bot — Sanal portföy botu ve canlı panosu
  → /stock-paper-bot/
- stock-analysis — Tek hisse için temel ve bilanço analizi
  → /stock-analysis/

Yeni proje eklemek HTML içinde tek bir kart bloğu eklemek kadar
kolay olmalı. Kart yapısını buna göre kur.

## Yapma
- Sayfaya veri çekme, durum gösterme, canlı içerik ekleme.
- Kart sayısı arttıkça filtreleme/arama gibi özellikler eklemeyi önerme.
