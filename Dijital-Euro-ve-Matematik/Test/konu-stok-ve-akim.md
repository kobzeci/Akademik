---
title: "Konu Notu — Stok ve Akım"
date: 2026-09-30
series: "Dijital Euro ve Matematik"
type: topic
tags:
  - stok
  - akim
  - bilanço
  - para
---

# Konu Notu — Stok ve Akım

## Temel ayrım

İktisadi modellemede **stok** belirli bir anda ölçülen büyüklüğü, **akım** ise belirli bir zaman aralığında gerçekleşen değişimi ifade eder.

### Stok örnekleri

- Bir bankanın 30 Eylül itibarıyla mevduat toplamı
- Merkez bankasının belirli bir tarihteki bilanço büyüklüğü
- Hanehalkının belirli bir gündeki dijital euro bakiyesi
- Kamu borç stoku

### Akım örnekleri

- Aylık gelir
- Yıllık vergi geliri
- Bir ay içinde verilen yeni krediler
- Bir dönem içinde dijital euroya dönüşen mevduat

## Basit ilişki

Bir stokun dönem sonu değeri şöyle yazılabilir:

\[
S_t = S_{t-1} + F_t
\]

### Semboller / Lejant

- **S_t**: t dönemindeki stok
- **S_{t-1}**: bir önceki dönemdeki stok
- **F_t**: dönem boyunca stoka eklenen net akım

Örneğin bir kullanıcının dijital euro bakiyesi dönem başında 500 euro ve dönem içinde net 120 euro artmışsa:

\[
DE_t = 500 + 120 = 620
\]

Bu ayrım özellikle bilanço-temelli para modelleri, Stock-Flow Consistent (SFC) modeller ve Dijital Euro'nun banka mevduatlarına etkisini analiz ederken temel olacaktır.

## Tez bağlantısı

Dijital Euro tartışmasında sık yapılan hatalardan biri, bir **stok değişimini** doğrudan yeni para yaratılması gibi yorumlamaktır.

Örneğin banka mevduatından dijital euroya 1.000 euro aktarılması:

- özel bankanın yükümlülük kompozisyonunu,
- merkez bankasının yükümlülük kompozisyonunu,
- ödeme sistemindeki bilanço ilişkilerini

değiştirebilir; ancak bunun toplam finansal serveti veya geniş para miktarını nasıl etkilediği ayrıca bilanço üzerinden analiz edilmelidir.

Bu nedenle ileride her modeli şu üç soruyla test edeceğiz:

1. Hangi büyüklük stok?
2. Hangi büyüklük akım?
3. İşlem sonrası hangi bilançonun hangi kalemi değişti?
