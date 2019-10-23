# Turkiye-AVM-Listesi

Türkiyedeki AVM'lerin bazı özellikleriyle birlikte , farklı formatlardaki listesi.

Avm ile ilgili aşağıdaki verileri içerir

- Adı
- Bulunduğu ilin plaka kodu
- Adresi
- Harita Linki (Regex ile içerisinden LAT,LNG Alınabilir)
- Shop sütununda ise virgüller ayrılarak içerisindeki mağazalar listelenmiştir.

### Basit Veri Sorgulama

Aşağıdaki basit sql sorgularıyla listede sorgulama yapabilirsiniz.

## Plakasına Göre Belirli Şehire Ait AVM'ler

`SELECT * FROM app_mall WHERE city_id = 16`

## Belirli şehirdeki Belirli mağazalar

`SELECT * FROM app_mall WHERE city_id = 16 AND shop LIKE '%atasun%'`

