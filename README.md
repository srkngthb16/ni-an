# Serkan & Melek — Nişan Davetiyesi

Mobil öncelikli, tek sayfalık dijital nişan davetiyesi. Ziyaretçilerin çoğu telefondan geleceği için tasarım telefona göre kurgulandı.

## Özellikler
- **Mühürlü davetiye açılışı** — sayfa açılınca zarf + wax mühür belirir; dokununca kapak 3D katlanır, mektup süzülür ve asıl site açılır.
- **Sinematik hero** — arka planda tam ekran video (poster ile hızlı ilk kare), çift isimleri, aile isimleri, tarih · mekân · saat.
- **Canlı geri sayım** — nişan gününe kalan gün / saat / dakika / saniye.
- **Otomatik akış** — site açılınca baştan sona ~33 saniyede kendiliğinden aşağı kayar; kullanıcı dokununca durur.
- **Bölümler** — Hikâye, Detaylar (Tarih / Saat / Mekân + harita), romantik ara söz, WhatsApp ile "Katılım Bildir".
- **1a paleti** — Krem · Altın · warm; tipografi Cormorant Garamond + Inter.

## Ayarlar
Etkinlik bilgileri `index.html` içindeki `CONFIG` bloğunda:

```js
const CONFIG = {
  eventISO:  "2026-08-16T19:00:00+03:00", // geri sayım hedefi
  dateText:  "16 Ağustos 2026 · Cumartesi",
  timeText:  "19.00",
  venue:     "Bahçe Restoran · Sarıyer, İstanbul",
  mapQuery:  "Bahçe Restoran Sarıyer İstanbul",
  whatsapp:  "900000000000",              // ülke kodu + numara
  scrollSeconds: 33
};
```

## Medya
`assets/` klasörü:
- `hero.mp4` / `hero.mov` — hero arka plan videosu
- `hero-poster.jpg` — video yüklenene kadar görünen kare

## Yayınlama
Statik site — kurulum gerektirmez. Klasörü Netlify / Vercel / GitHub Pages'e bırakmak yeterli.

## Teknoloji
Tek dosya `index.html` — vanilla HTML + CSS + JavaScript. Bağımlılık yok.
