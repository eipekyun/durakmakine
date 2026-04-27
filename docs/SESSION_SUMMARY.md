# Oturum Özeti

**Son güncelleme:** 2026-04-27

## Yapılanlar
- Proje iskelet dizini, [README.md](../README.md) ve [CLAUDE.md](../CLAUDE.md) kuruldu
- Genel belgeler: [firma](./firma.md), [ihtiyaçlar](./ihtiyaclar.md), [rakipler](./rakipler.md), [farklılaştırıcılar](./farklilastiricilar.md), [görüşmeler](./gorusmeler.md)
- Detaylı inceleme:
  - [Mevcut web tespitleri](./inceleme/mevcut-web.md) — WordPress, blog 2020'de ölü, talaşlı imalat sitede yok, alt linkler kırık
  - [Instagram durumu](./inceleme/instagram.md) — fetch sınırlı, manuel + toplantı kontrolü gerek
  - [Mekasis derinlemesine analiz](./inceleme/mekasis.md) — temsilcilikler güçlü, galeri placeholder, 5 eksen iddiası kanıtsız
  - [Sektör ve piyasa](./inceleme/sektor-piyasa.md) — Bursa otomotiv merkezi, Uysal ve NYT ek rakip, pres üreticileri iş ortağı potansiyeli
- [2026-04-28 toplantı hazırlık dokümanı](./toplanti/2026-04-28-hazirlik.md) — 19 soru + sunulacak bulgular + yeni site mimarisi taslağı
- **Müşteri sunumu üretildi:** [`scripts/build_sunum.py`](../scripts/build_sunum.py) → `cikti/durak-sunum.pptx` (12 slayt, lacivert + turuncu B2B palet, Mekasis vs Durak karşılaştırması, "Sözünü kanıtlayan üretici" ana mesajı)
- Git deposu başlatıldı, atomik commit'lerle ilk durum kaydedildi

## Sırada
1. **Yarınki telefon görüşmesi (2026-04-28)** — hazırlık dokümanı üzerinden ilerle
2. Toplantı notlarını [gorusmeler.md](./gorusmeler.md) altına `## 2026-04-28` başlığıyla işle
3. Netleşen bilgileri ilgili belgelere yansıt (yeni adres → firma.md, makine envanteri → farklılaştırıcılar.md, vb.)
4. Sunum içeriğini toplantı sonuçlarına göre güncelle (`scripts/build_sunum.py` düzenle → yeniden üret)
5. Bütçe ve scope onayı sonrası: teklif/sözleşme dokümanı

## Açık sorular (toplantıda kapatılacak)
- Yeni adres tam metni (GBP için)
- Tam makine envanteri (talaşlı imalat parkı)
- Diğer rakip firmalar (Uysal, NYT doğrulanacak + ek)
- Müşteri profili ve hedef coğrafya
- Domain/hosting/Instagram erişim sahipliği
- Foto/video arşivi var mı, çekim gerekli mi
- Bütçe ve hedef canlıya alınma tarihi
- Karar mekanizması (tek karar verici Fahrettin Bey mi?)
