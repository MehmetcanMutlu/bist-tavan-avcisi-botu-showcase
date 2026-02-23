# BIST Tavan Avcisi Botu (Showcase)

Bu repo, BIST Tavan Avcisi Botu adli dusuk gecikmeli park emir tetikleyici projesinin vitrin surumudur.

## Proje Ozeti
- Kullanicinin zaten acik olan internet bankaciligi oturumuna baglanma
- Login/form doldurma yapmadan sadece zamanli "Onayla" tetigi
- Hedef saatte milisaniye seviyesinde tetik icin iki asamali zamanlayici
- Dry-run modu ile tiklama atmadan zamanlama testi
- CLI override ile anlik parametre degistirme
- Selector Probe ile yari otomatik buton selector kesfi

## Teknoloji
- Python 3.11+
- Playwright (CDP attach)
- asyncio + perf_counter
- rich terminal UI
- pytest

## Guvenlik ve Kapsam Notu
- Bu depoda calisir kaynak kod yer almaz.
- Uretim kodu private depoda tutulur.
- Hicbir credential kaynak koda yazilmaz.
- Finansal sorumluluk kullaniciya aittir.

## Mimari
- `config.py`: merkezi ayar yonetimi
- `timing.py`: hedef zamani yakalama
- `browser.py`: mevcut tarayici oturumuna baglanma ve buton tetikleme
- `main.py`: orkestrasyon ve canli UI
- `dry_run.py`: tiklamasiz test
- `selector_probe.py`: olasi onay butonu selector adaylarini skorlama
- `price_calc.py`: BIST fiyat adimi/tavan hesaplamasi

## Durum
- Private repoda aktif gelistirme devam ediyor.
- Public repo yalnizca vitrin amaclidir (kaynak kod private tarafta).
