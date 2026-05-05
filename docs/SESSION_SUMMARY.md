# Oturum Özeti

**Son güncelleme:** 2026-05-05 (ofis ziyareti son dakika iptal, yeni randevu bekleniyor)
**Repo:** https://github.com/eipekyun/durakmakine
**Aşama:** 28 Nisan toplantı → post-mortem → strateji revize → 04 Mayıs müşteri dönüşü → **05 Mayıs ofis ziyareti müşteri tarafından iptal edildi**, alternatif zaman önerisi gelecek.

## Hemen sıradaki iş
**Pasif bekleme: müşteri 2 gün içinde alternatif zaman önerecek (kendi dediği).** Müşteri 2026-05-05 14:00 randevusundan 30 dk önce aradı, iş çıktığını söyledi. Saat sorunu olduğunu ima etti — akşam online veya gün içi başka vakit önerebilir.

ESMARK aksiyonu:
1. **2 gün bekle.** Müşterinin kendi geri dönmesini bekle, baskı yok.
2. **2026-05-07 Perşembe sabahı (10-11) hâlâ ses yoksa** kısa WhatsApp: "Müsait olduğunuz vakti söyleyin, online da olabilir, gün içi de" — **sadece saat sorulur, içerik konuşulmaz**.
3. **Akşam online tercih ederse** Google Meet linki + Calendar daveti hazırla; ofiste yüz yüze ısrar etme — müşterinin yükünü azalt.
4. Yeni randevu netleşene kadar [teklif-v2.md](./teklif-v2.md) ve qualifying soru hazırlığı sıcak tutulur — yeniden çıkartmaya gerek yok.

Detay ve hazırlık checklist: [gorusmeler.md → 2026-05-05 ofis ziyareti İPTAL](./gorusmeler.md).

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
