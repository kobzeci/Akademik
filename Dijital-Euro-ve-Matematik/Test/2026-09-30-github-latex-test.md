---
title: "GitHub LaTeX Testi — İktisadi Matematik"
date: 2026-09-30
series: "Dijital Euro ve Matematik"
type: test
tags:
  - latex
  - github
  - iktisadi-matematik
  - dijital-euro
---

# GitHub Uyumlu LaTeX Testi

Bu dosyanın amacı GitHub içinde matematiksel ifadelerin okunaklı biçimde render edilip edilmediğini test etmektir.

## 1. Basit denklem

Dijital euroya geçişin banka mevduatları üzerindeki basit etkisini şöyle yazalım:

$$
\Delta M_b = -\alpha \Delta DE
$$

### Semboller / Lejant

- $\Delta M_b$: banka mevduatındaki değişim
- $\Delta DE$: dijital euro miktarındaki değişim
- $\alpha$: mevduattan dijital euroya dönüşüm katsayısı

Eğer $\alpha = 0.8$ ve $\Delta DE = 100$ ise:

$$
\Delta M_b = -0.8 \times 100
$$

$$
\Delta M_b = -80
$$

Yani dijital euro miktarı 100 birim artarken banka mevduatı 80 birim azalır.

---

## 2. Kesirli ifade

Dönüşüm katsayısını doğrudan oran şeklinde de gösterebiliriz:

$$
\alpha = -\frac{\Delta M_b}{\Delta DE}
$$

Eğer banka mevduatı 60 azalırken dijital euro 100 artıyorsa:

$$
\alpha = -\frac{-60}{100}
$$

$$
\alpha = 0.6
$$

---

## 3. Fonksiyon gösterimi

Dijital euro talebini birkaç değişkenin fonksiyonu olarak düşünelim:

$$
DE_d = f(i, L, P, T)
$$

### Semboller / Lejant

- $DE_d$: dijital euro talebi
- $i$: faiz oranı
- $L$: likidite ihtiyacı
- $P$: mahremiyet tercihi
- $T$: teknolojiye güven düzeyi
- $f(\cdot)$: değişkenler arasındaki ilişkiyi gösteren fonksiyon

---

## 4. Türev testi

Faiz oranı yükseldiğinde dijital euro talebinin nasıl değiştiğini incelemek istersek:

$$
\frac{\partial DE_d}{\partial i} < 0
$$

Bu ifade, diğer değişkenler sabitken faiz oranı arttığında dijital euro talebinin azaldığını varsayar.

### Semboller / Lejant

- $\partial$: kısmi türev işareti
- $\frac{\partial DE_d}{\partial i}$: faiz oranındaki küçük bir değişimin dijital euro talebi üzerindeki marjinal etkisi

---

## 5. Zaman boyutu

Dijital euro stokunun dönemler arasındaki hareketini şöyle gösterebiliriz:

$$
DE_t = DE_{t-1} + I_t - O_t
$$

### Semboller / Lejant

- $DE_t$: t dönemindeki dijital euro stoku
- $DE_{t-1}$: bir önceki dönemdeki dijital euro stoku
- $I_t$: dönem içindeki dijital euro girişleri
- $O_t$: dönem içindeki dijital euro çıkışları

Örneğin:

$$
DE_{t-1} = 500
$$

$$
I_t = 150
$$

$$
O_t = 40
$$

ise:

$$
DE_t = 500 + 150 - 40 = 610
$$

---

## 6. Toplam işareti testi

Bir ekonomide tüm bireylerin dijital euro bakiyelerinin toplamı:

$$
DE^{total}_t = \sum_{j=1}^{N} DE_{j,t}
$$

### Semboller / Lejant

- $\sum$: toplama operatörü
- $j$: birey indeksi
- $N$: toplam birey sayısı
- $DE_{j,t}$: j bireyinin t dönemindeki dijital euro bakiyesi

---

## 7. Matris testi

İleride bilanço ilişkilerini matris biçiminde gösterebiliriz:

$$
\mathbf{x}_{t+1}
=
\begin{bmatrix}
M_{t+1} \\
DE_{t+1} \\
R_{t+1}
\end{bmatrix}
$$

ve basit bir geçiş sistemi:

$$
\mathbf{x}_{t+1} = A\mathbf{x}_t + \mathbf{u}_t
$$

### Semboller / Lejant

- $\mathbf{x}_t$: sistem durum vektörü
- $A$: geçiş matrisi
- $\mathbf{u}_t$: dışsal politika veya şok vektörü
- $R_t$: rezervler

---

## 8. İntegral testi

Sürekli zamanlı bir modelde bir akımın belirli bir zaman aralığındaki toplam etkisi:

$$
\Delta M = \int_{t_0}^{t_1} m(t)\,dt
$$

### Semboller / Lejant

- $\int$: integral işareti
- $t_0$: başlangıç zamanı
- $t_1$: bitiş zamanı
- $m(t)$: zamana bağlı para akımı

---

## Sonuç

Bu dosyada şu matematiksel gösterimler test edilmektedir:

- Yunan harfleri: $\alpha$, $\Delta$
- Alt indisler: $M_b$, $DE_t$
- Kesirler
- Kısmi türevler
- Toplam operatörü
- Matrisler
- İntegraller
- Satır içi matematik

Eğer GitHub sayfasında bunlar düzgün biçimde render ediliyorsa, günlük iktisadi matematik derslerini Markdown formatında tutabiliriz.
