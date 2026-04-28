# Oturum Özeti

**Son güncelleme:** 2026-04-28
**Repo:** https://github.com/eipekyun/durakmakine
**Aşama:** ESMARK Digital Marketing müşteri projesi — **toplantı tamamlandı, müşteri karar bekliyor**

## Hemen sıradaki iş
**Müşteri düşünme süreci.** 2026-04-28 telefon görüşmesi (~75 dk) yapıldı; teklif sözel olarak iletildi (web kurulum 20.000 TL + aylık 20.000 TL + ayrı reklam bütçesi). Onay gelene kadar:
1. Reklam bütçesi maliyet hesaplaması (sektörel benchmark + kanal dağılımı)
2. **5 metre torna** detayı yazılı olarak doğrulanmalı (boy mu çap mı — 27.04 yazışmasındaki "çap 780 × boy 5000" ile çelişiyor olabilir)
3. Onay gelirse: WhatsApp grubu + Drive klasörü kurulacak, 1 hafta içinde başlangıç, 2-3 haftada teslim

Toplantı detayı: [gorusmeler.md → 2026-04-28](./gorusmeler.md)

## Yapılanlar
- Proje iskelet dizini, [README.md](../README.md) ve [CLAUDE.md](../CLAUDE.md) kuruldu
- Genel belgeler: [firma](./firma.md), [ihtiyaçlar](./ihtiyaclar.md), [rakipler](./rakipler.md), [farklılaştırıcılar](./farklilastiricilar.md), [görüşmeler](./gorusmeler.md)
- Detaylı inceleme:
  - [Mevcut web tespitleri](./inceleme/mevcut-web.md) — WordPress, blog 2020'de ölü, talaşlı imalat sitede yok, alt linkler kırık
  - [Instagram durumu](./inceleme/instagram.md) — fetch sınırlı, manuel + toplantı kontrolü gerek
  - [Mekasis derinlemesine analiz](./inceleme/mekasis.md) — temsilcilikler güçlü, galeri placeholder, 5 eksen iddiası kanıtsız
  - [Sektör ve piyasa](./inceleme/sektor-piyasa.md) — Bursa otomotiv merkezi, Uysal ve NYT ek rakip, pres üreticileri iş ortağı potansiyeli
- [2026-04-28 toplantı hazırlık dokümanı](./toplanti/2026-04-28-hazirlik.md) yazıldı
- Müşteri sunumu üretildi: [`scripts/build_sunum.py`](../scripts/build_sunum.py) → `cikti/durak-sunum.pptx` (12 slayt, lacivert + turuncu B2B palet)
- **2026-04-28 telefon görüşmesi tamamlandı** — toplantı notu ve WhatsApp özeti [gorusmeler.md](./gorusmeler.md) altına işlendi
- Toplantıda netleşen bilgiler ilgili belgelere yansıtıldı:
  - [firma.md](./firma.md) — referanslar (Arçelik, Airpol, Betek Metal), %60-70 taşeronsuz, mekanik+hidrolik+otomasyon
  - [farklilastiricilar.md](./farklilastiricilar.md) — %60-70 oranı, referanslar bölümü

## Sonra (müşteri onayı geldikten sonra)
1. Reklam bütçesi teklifi netleştir → müşteri ile birlikte kanal dağılımı
2. Domain kontrolü, hosting devri, Instagram/Meta erişim, Google Business hesap devri
3. Foto/video çekim planı (mevcut arşivden çıkarılacak görseller + yeni çekim ihtiyacı)
4. Sözleşme/teklif dokümanı hazırla (`docs/teklif.md` oluştur)
5. Sunum içeriğini toplantı sonuçlarına göre güncelle (`scripts/build_sunum.py` düzenle)

## Açık doğrulamalar
- **5 metre torna** — boy mu çap mı (27.04 yazışmasındaki "çap 780 × boy 5000" ile uyumlu mu)
- Yeni adres tam metni (GBP için)
- Tam makine envanteri (talaşlı imalat parkı detayı)
- Diğer rakip firmalar (Uysal, NYT toplantıda netleşmedi — onay sonrası tekrar)
- Domain/hosting sahipliği bilgisi

## Geliştirme ortamı
- `.venv/` (gitignore'da) — `python -m venv .venv && .venv/bin/pip install python-pptx`
- Sunum üret: `.venv/bin/python scripts/build_sunum.py` → `cikti/durak-sunum.pptx`
