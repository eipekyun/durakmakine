# Oturum Özeti

**Son güncelleme:** 2026-04-28 (toplantı sonrası strateji revizyonu)
**Repo:** https://github.com/eipekyun/durakmakine
**Aşama:** Toplantı tamamlandı, **post-mortem yapıldı**, **strateji revize edildi**, müşteriye 5-7 gün sonra low-commitment paket ile dönülecek.

## Hemen sıradaki iş
**2026-05-05 Salı veya 2026-05-06 Çarşamba sabahı (10-11) takip mesajı.** Müşteri "düşüneceğim" pozisyonunda, aylık 20K paket ona fazla geldi. Pencere bu iki güne sıkışıyor çünkü:
- 05-01 Cuma → **1 Mayıs tatili**
- 05-02/03 → hafta sonu
- 05-04 Pzt → 1 Mayıs köprü günü (yarım/kapalı)

Yeni plan:
1. **7-8 gün sessiz bekleme** (müşterinin "düşünme zamanı" talebine saygı + baskı yokluğu sinyali, tatil penceresinden geç)
2. **Kısa WhatsApp mesajı** — taslak hazır: [gorusmeler.md → planlanan takip](./gorusmeler.md). Ton: müşteriyi haklı çıkar, aylık bağ olmadığını net söyle, detay isterse iletmek üzere kapıyı açık bırak.
3. **Müşteri detay isterse** revize teklif sunulur: [teklif-v2.md](./teklif-v2.md) — **15.000 TL tek seferlik**, web + GBP + temel SEO, aylık yönetim ve reklam yok.

## Toplantı post-mortem — özet
Detay: [post-mortem-2026-04-28.md](./post-mortem-2026-04-28.md). Ana bulgular:
- Müşteri 6 farklı yerde *"bu büyüklükte bir şeye hazır değilim"* dedi, iltifat sanıldı.
- *"Sizin web sayfasına değil, sisteme ihtiyacınız var"* cümlesi satışın bittiği an oldu.
- Çapraz referanslar (Akademi Döner, Bambini, Amerika 2-3K dolar) müşterinin ölçek kaygısını derinleştirdi.
- Bütçe konuşması toplantının %75'inde geldi — vizyon önce, fiyat sonra → "pahalıya patlar" yargısı oturmuş.
- Toplantı yapısı satıcı pozisyonuydu (sunum + plan); danışman pozisyonu (önce soru, sonra çözüm) gerekiyordu.
- **Gelecek toplantılar için 8 qualifying soru** ders defterinde — yüz yüze öncesi 15-20 dk telefonda sorulacak.

## Yapılanlar
- Proje iskelet, [README.md](../README.md), [CLAUDE.md](../CLAUDE.md)
- Genel belgeler: [firma](./firma.md), [ihtiyaçlar](./ihtiyaclar.md), [rakipler](./rakipler.md), [farklılaştırıcılar](./farklilastiricilar.md), [görüşmeler](./gorusmeler.md)
- İncelemeler: [mevcut-web](./inceleme/mevcut-web.md), [instagram](./inceleme/instagram.md), [mekasis](./inceleme/mekasis.md), [sektor-piyasa](./inceleme/sektor-piyasa.md)
- [2026-04-28 toplantı hazırlığı](./toplanti/2026-04-28-hazirlik.md)
- Müşteri sunumu: [`scripts/build_sunum.py`](../scripts/build_sunum.py) → `cikti/durak-sunum.pptx`
- **2026-04-28 telefon görüşmesi (~75 dk)** — notlar [gorusmeler.md](./gorusmeler.md) altına işlendi
- **Toplantı post-mortem ve ders defteri:** [post-mortem-2026-04-28.md](./post-mortem-2026-04-28.md)
- **Revize teklif paketi:** [teklif-v2.md](./teklif-v2.md) — 15.000 TL tek seferlik, low-commitment
- **Takip mesajı taslağı:** [gorusmeler.md](./gorusmeler.md) → planlanan iletişim (2026-05-03 ↔ 2026-05-05)

## Sonra (müşteri yanıtına göre dallanır)
- **Yanıt: "detay nedir?"** → teklif-v2 özeti gönder, görüşme öner; kabul ederse domain/hosting/erişim devri başlar
- **Yanıt: "şu an düşünmüyorum"** → kapıyı açık bırak; 2-3 ay sonra ışık dokunuş
- **Yanıt yok (1 hafta)** → tek bir sessiz değer paylaşımı; üçüncü mesaj yok

## Açık doğrulamalar (sözleşme öncesi)
- 5 metre torna ifadesinde "boy mu çap mı" — 27.04 yazışmasındaki "çap 780 × boy 5000 mm" ile tutarlılık
- Yeni adres tam metni (GBP için)
- Tam makine envanteri yazılı liste
- Referans müşteri (Arçelik, Airpol, Betek Metal) logo + isim kullanma izni
- Domain/hosting sahipliği bilgisi
- Foto/video arşivi durumu

## Geliştirme ortamı
- `.venv/` (gitignore'da) — `python -m venv .venv && .venv/bin/pip install python-pptx`
- Sunum üret: `.venv/bin/python scripts/build_sunum.py` → `cikti/durak-sunum.pptx`
