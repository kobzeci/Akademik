---
title: "İktisadi Matematiğe Giriş"
date: 2026-09-30
series: "Dijital Euro ve Matematik"
day: 1
type: lesson
tags:
  - iktisadi-matematik
  - dijital-euro
  - temel-kavramlar
---

# İktisadi Matematiğe Giriş — Gün 1

## Bugünkü amaç

İktisatta matematiğin neden kullanıldığını, bir ekonomik ilişkiyi sembollerle nasıl ifade ettiğimizi ve değişken–parametre ayrımını öğrenmek.

## 1. Matematik neden gerekli?

İktisat çoğu zaman şu tür sorular sorar:

- Gelir arttığında tüketim ne kadar artar?
- Faiz yükseldiğinde kredi talebi nasıl değişir?
- Bir merkez bankası bilançosundaki değişim özel sektörün bilançosunu nasıl etkiler?
- Dijital euroya geçiş banka mevduatlarını ne ölçüde değiştirir?

Bu ilişkileri yalnızca sözel olarak değil, açık ve test edilebilir biçimde ifade etmek için matematik kullanırız.

## 2. İlk ekonomik fonksiyon

Basit bir tüketim fonksiyonu:

\[
C = a + bY
\]

### Semboller / Lejant

- **C**: Toplam tüketim
- **a**: Gelir sıfır olsa bile yapılan otonom tüketim
- **b**: Marjinal tüketim eğilimi
- **Y**: Gelir

Örneğin:

\[
C = 100 + 0.8Y
\]

Gelir \(Y = 1{,}000\) ise:

\[
C = 100 + 0.8(1{,}000)
\]

Önce çarpma işlemi:

\[
0.8 \times 1{,}000 = 800
\]

Sonra otonom tüketimi ekleriz:

\[
C = 100 + 800 = 900
\]

Bu modelde 1.000 birimlik gelir 900 birimlik tüketime yol açar.

## 3. Değişken ve parametre

Fonksiyondaki **Y** bir değişkendir; farklı değerler alabilir.

Buna karşılık **a** ve **b**, model içinde kısa dönemde sabit kabul edilen parametrelerdir.

Bu ayrım ileride Dijital Euro modellerinde çok önemlidir. Örneğin:

\[
D = f(i, L, P)
\]

### Semboller / Lejant

- **D**: Dijital euro talebi
- **i**: Faiz oranı
- **L**: Likidite ihtiyacı
- **P**: Mahremiyet tercihi
- **f(·)**: Bu değişkenleri dijital euro talebine bağlayan fonksiyon

Burada amaç henüz fonksiyonun tam biçimini bilmek değil; ekonomik bir düşünceyi matematiksel bir yapıya çevirmeyi öğrenmektir.

## 4. Dijital Euro bağlantısı

Tez çalışmasında ileride şu tür sorular matematiksel modellere dönüşebilir:

\[
\Delta M_b = -\alpha \Delta DE
\]

### Semboller / Lejant

- **Δ**: Değişim
- **M_b**: Banka mevduatı
- **DE**: Dijital euro miktarı
- **α**: Dijital euroya geçen her 1 birimin banka mevduatından ne kadar çekildiğini gösteren katsayı

Örneğin \(\alpha = 1\) ise 100 euro dijital euroya geçiş banka mevduatını 100 euro azaltır.

Ama \(\alpha < 1\) ise bunun bir kısmı nakitten veya başka finansal varlıklardan geliyor olabilir.

İlerleyen derslerde bu tür denklemleri bilanço mantığıyla birlikte kuracağız.

## 5. Bugünün özeti

Bugün üç temel fikir öğrendik:

1. Matematik ekonomik ilişkileri açık biçimde ifade eder.
2. Değişkenler model içinde değişir; parametreler belirli bir analiz için sabit kabul edilir.
3. Bir ekonomik düşünce önce basit bir fonksiyona, daha sonra daha gelişmiş bir modele dönüştürülebilir.

## Mini soru

\[
C = 50 + 0.75Y
\]

ve \(Y = 800\) ise tüketim **C** kaçtır?

Cevabı bir sonraki tartışmada birlikte kontrol edeceğiz.
