# Gün 21 — Dinamik Sermaye, Yatırım ve Kapasite

## Amaçlı Dijital Euro yalnızca bugünkü talebi değil, yarının üretim kapasitesini de artırabilir mi?

Gün 20'de şu statik çerçeveyi kurduk:

$$
G_t=Y_t^*-Y_t
$$

### Semboller / Lejant

- $G_t$: $t$ dönemindeki kapasite veya çıktı açığı.
- $Y_t^*$: $t$ dönemindeki potansiyel üretim.
- $Y_t$: $t$ dönemindeki fiilî üretim.
- $t$: Zaman indeksi.

Aynı derste amaçlı Dijital Euro'nun oluşturduğu talebi:

$$
D_t=b(1-s_t)I_t
$$

### Semboller / Lejant

- $D_t$: $t$ dönemindeki ilave nihai talep.
- $b$: Net paranın harcamaya dönüşme oranı.
- $s_t$: $t$ dönemindeki sterilizasyon oranı.
- $I_t$: $t$ dönemindeki brüt amaçlı Dijital Euro ihracı.

ve kapasiteyi aşan talebi:

$$
E_t=\max(0,D_t-G_t)
$$

### Semboller / Lejant

- $E_t$: Kapasiteyi aşan fazla talep.
- $\max(0,D_t-G_t)$: $D_t-G_t$ negatifse sıfır, pozitifse pozitif farkı alan ifade.
- $D_t$: İlave talep.
- $G_t$: Mevcut kapasite açığı.

olarak yazmıştık.

Bu yaklaşım önemliydi ama eksikti. Çünkü potansiyel üretimi $Y_t^*$ sabit kabul ediyorduk.

Bugün bu varsayımı kaldırıyoruz.

Temel sorumuz:

> Amaçlı Dijital Euro tüketimi değil üretken yatırımı finanse ederse, bugünkü para yaratımı yarının kapasitesini büyütebilir mi?

Bu soru tez açısından kritik. Çünkü amaçlı para yalnızca mevcut kapasiteyi kullanıyorsa geçici bir talep aracı olur. Fakat yeni sermaye oluşturuyorsa, sistemin arz tarafını da değiştirebilir.

---

## 1. Stok ve akım ayrımı

Önce çok temel bir ayrım yapalım.

Sermaye:

$$
K_t
$$

### Semboller / Lejant

- $K_t$: $t$ dönemindeki sermaye stoku.
- Stok: Belirli bir anda ölçülen büyüklük.

bir **stoktur**.

Yatırım ise:

$$
J_t
$$

### Semboller / Lejant

- $J_t$: $t$ dönemi boyunca yapılan reel yatırım.
- Akım: Belirli bir zaman aralığında gerçekleşen büyüklük.

bir **akımdır**.

Örneğin bir fabrikanın toplam makine parkı bir stoktur. Bu yıl satın alınan yeni makineler ise akımdır.

Bu ayrım ileride SFC — **Stock-Flow Consistent (Stok-Akım Tutarlı)** modellerde temel olacak.

---

## 2. Sermaye birikim denklemi

Bir ekonomide gelecek dönem sermaye stoku, bugünkü sermayenin amortisman sonrası kalan kısmı ile yeni yatırımın toplamıdır:

$$
K_{t+1}=(1-\delta)K_t+J_t
$$

### Semboller / Lejant

- $K_{t+1}$: Bir sonraki dönemin sermaye stoku.
- $K_t$: Mevcut sermaye stoku.
- $\delta$: Sermayenin amortisman oranı.
- $1-\delta$: Sermayenin dönem sonunda ayakta kalan oranı.
- $J_t$: Dönem içindeki yeni reel yatırım.

Bu denklem dinamik iktisadın en temel hareket denklemlerinden biridir.

---

## 3. Denklem neden böyle?

Diyelim ki mevcut sermaye:

$$
K_t=200
$$

### Semboller / Lejant

- $K_t$: Başlangıç sermaye stoku.

ve amortisman oranı:

$$
\delta=0.05
$$

### Semboller / Lejant

- $\delta=0.05$: Sermayenin yüzde 5'inin dönem içinde ekonomik veya fiziksel olarak aşınması.

olsun.

Dönem sonunda mevcut sermayenin kalan kısmı:

$$
(1-\delta)K_t
$$

### Semboller / Lejant

- $1-\delta$: Sermayenin kalan oranı.
- $K_t$: Başlangıç sermayesi.

Yerine koyarsak:

$$
(1-0.05)200
$$

### Semboller / Lejant

- $0.95$: Sermayenin yüzde 95'inin kaldığını gösterir.
- $200$: Başlangıç sermaye stoku.

$$
0.95\times200=190
$$

### Semboller / Lejant

- $190$: Amortisman sonrası kalan sermaye.

Eğer yeni yatırım:

$$
J_t=20
$$

### Semboller / Lejant

- $J_t$: Dönem içinde yapılan yeni yatırım.

ise:

$$
K_{t+1}=190+20
$$

### Semboller / Lejant

- $K_{t+1}$: Yeni dönem sermaye stoku.
- $190$: Eski sermayenin kalan kısmı.
- $20$: Yeni yatırım.

ve:

$$
K_{t+1}=210
$$

### Semboller / Lejant

- $210$: Bir sonraki dönemin toplam sermaye stoku.

olur.

---

## 4. Net yatırım nedir?

Sermaye stokundaki değişimi:

$$
\Delta K_t=K_{t+1}-K_t
$$

### Semboller / Lejant

- $\Delta K_t$: Sermaye stokundaki dönemsel değişim.
- $K_{t+1}$: Gelecek dönem sermaye stoku.
- $K_t$: Mevcut sermaye stoku.

olarak tanımlayalım.

Sermaye birikim denklemimizi yerine koyalım:

$$
\Delta K_t=(1-\delta)K_t+J_t-K_t
$$

### Semboller / Lejant

- $\Delta K_t$: Net sermaye artışı.
- $\delta K_t$: Amortisman nedeniyle kaybedilen sermaye.
- $J_t$: Brüt yeni yatırım.

Benzer terimleri düzenleyelim:

$$
\Delta K_t=J_t-\delta K_t
$$

### Semboller / Lejant

- $J_t$: Brüt yatırım.
- $\delta K_t$: Amortisman.
- $J_t-\delta K_t$: Net yatırım.

Bu çok önemli bir sonuçtur:

> Sermaye stokunun artması için yeni yatırımın yalnızca pozitif olması yetmez; amortismanı aşması gerekir.

Yani:

$$
J_t>\delta K_t
$$

### Semboller / Lejant

- $J_t$: Yeni yatırım.
- $\delta K_t$: Mevcut sermayenin aşınan kısmı.

ise:

$$
\Delta K_t>0
$$

### Semboller / Lejant

- $\Delta K_t>0$: Sermaye stoku büyüyor.

olur.

---

## 5. Amaçlı Dijital Euro yatırımı nasıl finanse eder?

Şimdi tez bağlantısını kuralım.

Sterilizasyon sonrası ekonomide kalan amaçlı para:

$$
P_t^{net}=(1-s_t)I_t
$$

### Semboller / Lejant

- $P_t^{net}$: Ekonomide etkili kalan net amaçlı para.
- $s_t$: Sterilizasyon oranı.
- $I_t$: Brüt amaçlı Dijital Euro ihracı.

Bu net paranın tamamının reel yatırıma dönüşmediğini varsayalım.

Yatırıma dönüşme oranı:

$$
\beta
$$

### Semboller / Lejant

- $\beta$: Net amaçlı paranın reel yatırıma dönüşen oranı.
- $0\leq\beta\leq1$: Oranın sıfır ile bir arasında olduğunu gösterir.

olsun.

O zaman amaçlı para ile finanse edilen yatırım:

$$
J_t=\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $J_t$: Reel yatırım.
- $\beta$: Net paranın yatırıma dönüşüm oranı.
- $s_t$: Sterilizasyon oranı.
- $I_t$: Brüt amaçlı ihraç.

Bu denklem para ile reel sermaye arasındaki ilk köprümüzdür.

---

## 6. Para ihracını sermaye hareket denklemine yerleştirelim

Başlangıç denklemimiz:

$$
K_{t+1}=(1-\delta)K_t+J_t
$$

### Semboller / Lejant

- $K_{t+1}$: Gelecek sermaye stoku.
- $K_t$: Mevcut sermaye stoku.
- $\delta$: Amortisman oranı.
- $J_t$: Yeni yatırım.

Şimdi:

$$
J_t=\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $\beta(1-s_t)I_t$: Amaçlı Dijital Euro'dan reel yatırıma dönüşen miktar.

ifadesini yerine koyalım:

$$
K_{t+1}=(1-\delta)K_t+\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $K_{t+1}$: Bir sonraki dönem sermaye stoku.
- $(1-\delta)K_t$: Eski sermayenin kalan kısmı.
- $\beta(1-s_t)I_t$: Amaçlı Dijital Euro ile finanse edilen yeni reel yatırım.

Bu, tez modelimizin ilk gerçek dinamik para-sermaye denklemidir.

---

## 7. İhraç miktarının gelecek sermayeye marjinal etkisi

Şimdi $I_t$ bir birim arttığında $K_{t+1}$ ne kadar değişir?

Denklem:

$$
K_{t+1}=(1-\delta)K_t+\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $I_t$: Politika aracımız olan brüt ihraç.
- $K_{t+1}$: Sonraki dönem sermaye stoku.

$I_t$'ye göre kısmi türev alalım:

$$
\frac{\partial K_{t+1}}{\partial I_t}=\beta(1-s_t)
$$

### Semboller / Lejant

- $\frac{\partial K_{t+1}}{\partial I_t}$: Bir birim ek ihraç nedeniyle gelecek dönem sermaye stokundaki marjinal değişim.
- $\beta$: Yatırıma dönüşüm oranı.
- $1-s_t$: Sterilizasyon sonrası kalan oran.

Bu sonuç sezgiseldir.

Örneğin:

$$
\beta=0.60
$$

### Semboller / Lejant

- $\beta=0.60$: Net paranın yüzde 60'ı reel yatırıma dönüşüyor.

ve:

$$
s_t=0.20
$$

### Semboller / Lejant

- $s_t=0.20$: Brüt ihracın yüzde 20'si sterilize ediliyor.

ise:

$$
\frac{\partial K_{t+1}}{\partial I_t}=0.60(0.80)
$$

### Semboller / Lejant

- $0.80$: Ekonomide kalan oran.

$$
\frac{\partial K_{t+1}}{\partial I_t}=0.48
$$

### Semboller / Lejant

- $0.48$: Bir birim ek brüt ihracın gelecek dönem sermaye stokunu 0.48 birim artırdığı basitleştirilmiş sonuç.

---

## 8. Sermayeden potansiyel üretime geçiş

Şimdi sermaye stokunu üretim kapasitesine bağlayalım.

İlk basit yaklaşım:

$$
Y_t^*=\kappa K_t
$$

### Semboller / Lejant

- $Y_t^*$: Potansiyel üretim.
- $K_t$: Sermaye stoku.
- $\kappa$: Bir birim sermayenin potansiyel üretime katkısını gösteren kapasite katsayısı.

Bu model şimdilik emeği, teknolojiyi ve diğer girdileri sabit kabul ediyor.

Bir sonraki dönemde:

$$
Y_{t+1}^*=\kappa K_{t+1}
$$

### Semboller / Lejant

- $Y_{t+1}^*$: Bir sonraki dönemin potansiyel üretimi.
- $K_{t+1}$: Bir sonraki dönem sermaye stoku.
- $\kappa$: Kapasite dönüşüm katsayısı.

---

## 9. Para ihracını doğrudan gelecekteki kapasiteye bağlayalım

Az önce:

$$
K_{t+1}=(1-\delta)K_t+\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $K_{t+1}$: Gelecek sermaye stoku.
- $\beta(1-s_t)I_t$: Amaçlı para ile finanse edilen yatırım.

bulmuştuk.

Bunu potansiyel üretim denklemine koyalım:

$$
Y_{t+1}^*=\kappa\left[(1-\delta)K_t+\beta(1-s_t)I_t\right]
$$

### Semboller / Lejant

- $Y_{t+1}^*$: Gelecek dönem üretim kapasitesi.
- $\kappa$: Sermayeyi potansiyel üretime çeviren katsayı.
- $(1-\delta)K_t$: Korunan eski sermaye.
- $\beta(1-s_t)I_t$: Yeni üretken yatırım.

Parantezi açarsak:

$$
Y_{t+1}^*=\kappa(1-\delta)K_t+\kappa\beta(1-s_t)I_t
$$

### Semboller / Lejant

- İlk terim: Mevcut sermayeden kalan üretim kapasitesi.
- İkinci terim: Amaçlı Dijital Euro'nun yeni kapasite katkısı.

Şimdi $I_t$'ye göre türev alalım:

$$
\frac{\partial Y_{t+1}^*}{\partial I_t}=\kappa\beta(1-s_t)
$$

### Semboller / Lejant

- $\frac{\partial Y_{t+1}^*}{\partial I_t}$: Bugünkü bir birim ek ihracın yarının potansiyel üretimine marjinal etkisi.
- $\kappa$: Sermayenin kapasite üretkenliği.
- $\beta$: Paranın yatırıma dönüşme oranı.
- $1-s_t$: Sterilizasyon sonrası kalan oran.

Bu, bugünkü dersin tez açısından en önemli denklemlerinden biridir.

---

## 10. Tüketim amaçlı para ile yatırım amaçlı para arasındaki fark

Şimdi iki farklı kullanım düşünelim.

Birinci kullanım, doğrudan tüketim talebi yaratıyor:

$$
D_t^C=b_C(1-s_t)I_t^C
$$

### Semboller / Lejant

- $D_t^C$: Tüketim kanalından oluşan ilave talep.
- $b_C$: Tüketim harcamasına dönüşüm oranı.
- $I_t^C$: Tüketim amaçlı brüt ihraç.
- Üst indis $C$: Consumption, yani tüketim.

İkinci kullanım yatırım yaratıyor:

$$
J_t=\beta(1-s_t)I_t^J
$$

### Semboller / Lejant

- $J_t$: Reel yatırım.
- $I_t^J$: Yatırım amaçlı brüt ihraç.
- Üst indis $J$: Yatırım kanalını gösteren etiket.
- $\beta$: Yatırıma dönüşüm oranı.

Tüketim amaçlı para mevcut kapasiteyi kullanır.

Yatırım amaçlı para ise başarılıysa gelecek kapasiteyi artırır.

Bu ayrım senin çok katmanlı Dijital Euro fikrin için temel olabilir.

---

## 11. Yatırımın zamanlama problemi

Burada önemli bir sorun var.

Amaçlı para bugün çıkar:

$$
I_t>0
$$

### Semboller / Lejant

- $I_t$: Bugünkü brüt ihraç.

fakat yeni kapasite çoğu zaman hemen oluşmaz.

Basitçe bir dönem gecikme varsayarsak:

$$
I_t\rightarrow J_t\rightarrow K_{t+1}\rightarrow Y_{t+1}^*
$$

### Semboller / Lejant

- Oklar: Nedensel/zamansal aktarım sırasını gösterir.
- $J_t$: Bugünkü yatırım.
- $K_{t+1}$: Yarınki sermaye.
- $Y_{t+1}^*$: Yarınki üretim kapasitesi.

Bu nedenle yatırım amaçlı para kısa vadede yine talep yaratırken arz etkisi daha geç gelebilir.

Bu gecikme enflasyon açısından kritik olabilir.

---

## 12. Bugünkü talep ile yarınki kapasiteyi birlikte yazmak

Amaçlı para bugün yatırım mallarına talep oluştursun:

$$
D_t^J=b_J(1-s_t)I_t
$$

### Semboller / Lejant

- $D_t^J$: Yatırım kaynaklı bugünkü talep.
- $b_J$: İhraçtan yatırım malı talebine dönüşüm oranı.
- $s_t$: Sterilizasyon oranı.
- $I_t$: Brüt ihraç.

Aynı para yarın kapasite oluştursun:

$$
\Delta Y_{t+1}^*=\kappa\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $\Delta Y_{t+1}^*$: Gelecek dönem potansiyel üretimdeki artış.
- $\kappa$: Sermayenin kapasite katsayısı.
- $\beta$: Yatırıma dönüşüm oranı.
- $1-s_t$: Net kalan para oranı.
- $I_t$: Brüt ihraç.

Bu iki denklem politika tasarımındaki temel gerilimi gösterir:

> Aynı yatırım programı bugün talep baskısı yaratırken yarın arz kapasitesini artırabilir.

---

## 13. Kapasite açığının dinamik hale gelmesi

Gün 20'de:

$$
G_t=Y_t^*-Y_t
$$

### Semboller / Lejant

- $G_t$: Bugünkü kapasite açığı.
- $Y_t^*$: Potansiyel üretim.
- $Y_t$: Fiilî üretim.

demiştik.

Bir sonraki dönem:

$$
G_{t+1}=Y_{t+1}^*-Y_{t+1}
$$

### Semboller / Lejant

- $G_{t+1}$: Gelecek dönem kapasite açığı.
- $Y_{t+1}^*$: Gelecek potansiyel üretim.
- $Y_{t+1}$: Gelecek fiilî üretim.

Artık $Y_{t+1}^*$ sabit değil:

$$
Y_{t+1}^*=\kappa\left[(1-\delta)K_t+\beta(1-s_t)I_t\right]
$$

### Semboller / Lejant

- $I_t$: Bugünkü politika kararının gelecekte kapasiteyi değiştirdiğini gösterir.

Dolayısıyla bugünkü para politikası gelecekteki kapasite açığını da değiştirir.

---

## 14. Statik model ile dinamik model arasındaki fark

Statik model şu soruyu sorar:

> Bugün 10 birim daha para verirsek bugünkü üretim ve fiyat ne olur?

Dinamik model ise şunu sorar:

> Bugün 10 birim daha para verirsek bugün ne olur, yarın sermaye ne kadar artar, gelecek kapasite nasıl değişir ve sonraki dönem enflasyon baskısı nasıl etkilenir?

Matematiksel olarak statik ilişki:

$$
Y=f(I)
$$

### Semboller / Lejant

- $Y$: Aynı dönem sonucu.
- $I$: Politika girdisi.

iken dinamik ilişki:

$$
K_{t+1}=f(K_t,I_t)
$$

### Semboller / Lejant

- $K_{t+1}$: Gelecek dönem durum değişkeni.
- $K_t$: Mevcut durum.
- $I_t$: Bugünkü politika girdisi.

biçimindedir.

---

## 15. Durum değişkeni ve kontrol değişkeni

Kontrol teorisine hazırlık için iki kavram öğrenelim.

Sermaye:

$$
K_t
$$

### Semboller / Lejant

- $K_t$: Sistemin geçmiş kararlarının sonucunu taşıyan durum değişkeni.

bir **durum değişkenidir**.

İhraç:

$$
I_t
$$

### Semboller / Lejant

- $I_t$: Politika yapıcının dönem içinde seçebildiği kontrol değişkeni.

ise bir **kontrol değişkenidir**.

Sterilizasyon oranı:

$$
s_t
$$

### Semboller / Lejant

- $s_t$: Politika yapıcının ikinci kontrol aracı.

da kontrol değişkeni olabilir.

Bu dil ileride kontrol teorisinde doğrudan kullanılacak.

---

## 16. Basit iki kontrol aracı

Dinamik sermaye denklemimiz:

$$
K_{t+1}=(1-\delta)K_t+\beta(1-s_t)I_t
$$

### Semboller / Lejant

- Durum değişkeni: $K_t$.
- Kontrol değişkenleri: $I_t$ ve $s_t$.
- Parametreler: $\delta$ ve $\beta$.

Politika yapıcı aynı net yatırım etkisini farklı kombinasyonlarla üretebilir.

Örneğin yüksek:

$$
I_t
$$

### Semboller / Lejant

- $I_t$: Brüt ihraç.

ve yüksek:

$$
s_t
$$

### Semboller / Lejant

- $s_t$: Sterilizasyon oranı.

veya daha düşük ihraç ile daha düşük sterilizasyon kullanılabilir.

Ancak iki politikanın bankacılık, bilanço, beklenti ve likidite etkileri aynı olmayabilir.

Bu ileride SFC ve bankacılık modeline eklenmelidir.

---

## 17. Durağan durum fikri

Dinamik sistemlerde önemli bir kavram **steady state — durağan durum**dur.

Sermaye stokunun değişmediği durumda:

$$
K_{t+1}=K_t=K^*
$$

### Semboller / Lejant

- $K^*$: Durağan durum sermaye stoku.
- $K_{t+1}=K_t$: Sermayenin dönemden döneme değişmediği durum.

Sermaye denklemine yazalım:

$$
K^*=(1-\delta)K^*+J
$$

### Semboller / Lejant

- $J$: Sabit kabul edilen yatırım akımı.
- $\delta$: Amortisman oranı.

Sağ taraftaki sermaye terimini sola alalım:

$$
K^*-(1-\delta)K^*=J
$$

### Semboller / Lejant

- Sol taraf: Sermayenin korunması için gereken net fark.

Paranteze alalım:

$$
K^*\left[1-(1-\delta)\right]=J
$$

### Semboller / Lejant

- Köşeli ifade burada yalnızca cebirsel gruplamayı gösterir; GitHub formül gösteriminde normal LaTeX kullanılmıştır.

İç ifadeyi sadeleştirelim:

$$
1-(1-\delta)=\delta
$$

### Semboller / Lejant

- $\delta$: Amortisman oranı.

Dolayısıyla:

$$
\delta K^*=J
$$

### Semboller / Lejant

- $\delta K^*$: Durağan durumda aşınan sermaye miktarı.
- $J$: Bu aşınmayı tam olarak telafi eden yatırım.

Buradan:

$$
K^*=\frac{J}{\delta}
$$

### Semboller / Lejant

- $K^*$: Durağan durum sermaye stoku.
- $J$: Sabit yatırım.
- $\delta$: Amortisman oranı.

Bu sonuç çok sezgiseldir:

> Uzun vadede sermaye stokunun sabit kalması için yatırım, amortismanı tam karşılamalıdır.

---

## 18. Amaçlı Dijital Euro ile durağan durum sermayesi

Eğer yatırım:

$$
J=\beta(1-s)I
$$

### Semboller / Lejant

- $\beta$: Yatırıma dönüşüm oranı.
- $s$: Sabit sterilizasyon oranı.
- $I$: Sabit brüt ihraç.

ise durağan durum:

$$
K^*=\frac{\beta(1-s)I}{\delta}
$$

### Semboller / Lejant

- $K^*$: Uzun dönem sermaye stoku.
- $\beta(1-s)I$: Amaçlı paradan gelen sürekli yatırım akımı.
- $\delta$: Amortisman oranı.

Bu ifade güçlüdür ama dikkatle yorumlanmalıdır.

Sürekli para ihracının gerçekten sürekli reel yatırım yaratabileceğini varsayıyoruz. Gerçek sistemde finansman talebi, proje kalitesi, işgücü, teknoloji, ithalat ve enflasyon kısıtları bu ilişkiyi sınırlar.

---

## 19. Yatırım kalitesi: her sermaye artışı aynı değildir

Şimdi önemli bir ayrım daha ekleyelim.

Amaçlı para 100 birim yatırım yaratabilir, fakat bu yatırımın verimliliği düşük olabilir.

Bu nedenle:

$$
Y_t^*=\kappa K_t
$$

### Semboller / Lejant

- $\kappa$: Sermayenin üretkenlik katsayısı.

denklemindeki $\kappa$ çok önemlidir.

İki proje aynı sermaye tutarını yaratabilir:

$$
\Delta K_A=\Delta K_B
$$

### Semboller / Lejant

- $\Delta K_A$: A projesinin oluşturduğu sermaye.
- $\Delta K_B$: B projesinin oluşturduğu sermaye.

ama:

$$
\kappa_A>\kappa_B
$$

### Semboller / Lejant

- $\kappa_A$: A yatırımının üretkenlik katsayısı.
- $\kappa_B$: B yatırımının üretkenlik katsayısı.

ise A projesi daha fazla üretim kapasitesi yaratır.

Dolayısıyla amaçlı Dijital Euro tasarımında yalnızca “yatırım yapıldı mı?” değil:

> Bir euro finansman başına ne kadar üretken kapasite yaratıldı?

sorusu önemlidir.

---

## 20. Sermaye yaratımının ithalat boyutu

Yeni yatırımın bir kısmı ithal makine ve teknoloji gerektiriyorsa:

$$
M_t^K=m_KJ_t
$$

### Semboller / Lejant

- $M_t^K$: Sermaye yatırımından kaynaklanan ithalat.
- $m_K$: Yatırımın ithalat yoğunluğu.
- $J_t$: Reel yatırım.

Amaçlı para denklemimizi koyarsak:

$$
M_t^K=m_K\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $m_K$: Yatırımın döviz/ithalat sızıntısı.
- $\beta(1-s_t)I_t$: Amaçlı paradan oluşan yatırım.

Bu nedenle yüksek kapasite yaratımı bile kısa vadede dış denge baskısı oluşturabilir.

Tez modelinin ileride aynı anda en az üç sonucu izlemesi gerekir:

$$
\Delta K_t,\quad \Delta\pi_t,\quad M_t
$$

### Semboller / Lejant

- $\Delta K_t$: Sermaye artışı.
- $\Delta\pi_t$: Enflasyon değişimi.
- $M_t$: İthalat ihtiyacı.

---

## 21. Basit bir dinamik politika amacı

İleride politika yapıcıyı şöyle düşünebiliriz:

$$
W_t=\omega_K\Delta K_t-\omega_\pi(\Delta\pi_t)^2-\omega_M M_t
$$

### Semboller / Lejant

- $W_t$: $t$ dönemindeki politika değeri.
- $\omega_K$: Sermaye/kapasite artışına verilen ağırlık.
- $\omega_\pi$: Enflasyon maliyetine verilen ağırlık.
- $\omega_M$: İthalat maliyetine verilen ağırlık.
- $(\Delta\pi_t)^2$: Büyük enflasyon sapmalarını daha ağır cezalandıran terim.

Bu henüz nihai tez modeli değildir. Fakat artık politika sorusu yalnızca bugünkü büyüme değil:

> Bugünkü enflasyon ve dış denge maliyeti karşılığında gelecekte ne kadar üretken kapasite kazanıyoruz?

haline gelir.

---

## 22. Küçük türetme: sterilizasyon gelecek kapasiteyi nasıl etkiler?

Temel denklem:

$$
Y_{t+1}^*=\kappa(1-\delta)K_t+\kappa\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $Y_{t+1}^*$: Gelecek potansiyel üretim.
- $s_t$: Sterilizasyon oranı.
- $I_t$: Brüt ihraç.

$s_t$'ye göre türev alalım:

$$
\frac{\partial Y_{t+1}^*}{\partial s_t}
=
-\kappa\beta I_t
$$

### Semboller / Lejant

- $\frac{\partial Y_{t+1}^*}{\partial s_t}$: Sterilizasyon oranındaki küçük artışın gelecek kapasite üzerindeki marjinal etkisi.
- Eksi işareti: Diğer koşullar aynıyken daha yüksek sterilizasyonun yatırım kanalını azaltabileceğini gösterir.

Eğer:

$$
\kappa>0,\quad \beta>0,\quad I_t>0
$$

### Semboller / Lejant

- Tüm katsayıların pozitif olduğu normal durum.

ise:

$$
\frac{\partial Y_{t+1}^*}{\partial s_t}<0
$$

### Semboller / Lejant

- Sonuç: Daha yüksek sterilizasyon, bu basit modelde gelecekteki kapasite artışını azaltır.

Bu çok önemli bir politika gerilimidir.

Gün 20'de sterilizasyonun bugünkü enflasyon baskısını azaltabileceğini gördük.

Bugün ise aşırı sterilizasyonun gelecekteki kapasite oluşumunu da azaltabileceğini görüyoruz.

Yani optimal sterilizasyon:

> mümkün olan en yüksek sterilizasyon

değil, bugünkü fiyat istikrarı ile yarının kapasite artışı arasında denge kuran bir oran olmalıdır.

---

## 23. Tez için ilk dinamik zincir

Bugünkü bütün sistemi tek bir akışta yazalım:

$$
I_t
\rightarrow
(1-s_t)I_t
\rightarrow
J_t
\rightarrow
K_{t+1}
\rightarrow
Y_{t+1}^*
\rightarrow
G_{t+1}
$$

### Semboller / Lejant

- $I_t$: Brüt amaçlı Dijital Euro ihracı.
- $(1-s_t)I_t$: Sterilizasyon sonrası net para.
- $J_t$: Reel yatırım.
- $K_{t+1}$: Gelecek sermaye stoku.
- $Y_{t+1}^*$: Gelecek potansiyel üretim.
- $G_{t+1}$: Gelecek kapasite açığı.

Bu zincir, tezindeki “reel değer yaratımı” fikrinin dinamik çekirdeğini oluşturabilir.

---

## 24. Bugünün ana fikri

Gün 20'de kapasiteyi sabit bir tavan olarak ele almıştık.

Bugün kapasitenin yatırım yoluyla değişebileceğini öğrendik.

Temel hareket denklemi:

$$
K_{t+1}=(1-\delta)K_t+\beta(1-s_t)I_t
$$

### Semboller / Lejant

- $K_{t+1}$: Gelecek sermaye.
- $\delta$: Amortisman.
- $\beta$: Yatırıma dönüşüm oranı.
- $s_t$: Sterilizasyon oranı.
- $I_t$: Brüt amaçlı ihraç.

Potansiyel üretim:

$$
Y_{t+1}^*=\kappa K_{t+1}
$$

### Semboller / Lejant

- $Y_{t+1}^*$: Gelecek üretim kapasitesi.
- $\kappa$: Sermayenin üretkenlik katsayısı.

ve amaçlı paranın gelecek kapasite üzerindeki marjinal etkisi:

$$
\frac{\partial Y_{t+1}^*}{\partial I_t}
=
\kappa\beta(1-s_t)
$$

### Semboller / Lejant

- Sonuç: Amaçlı para ancak sterilizasyon sonrası ekonomide kalır, yatırıma dönüşür ve üretken sermaye oluşturursa gelecekteki kapasiteyi artırır.

Bugünün temel tez mesajı şudur:

> Amaçlı Dijital Euro'nun başarısını yalnızca aynı dönemde yarattığı talep ve enflasyonla değil, gelecekte oluşturduğu üretken sermaye ve kapasiteyle birlikte değerlendirmek gerekir.

Bir sonraki derste bu hareket denklemini kullanarak **birinci dereceden fark denklemlerine**, zaman içindeki yakınsama/uzaklaşma mantığına ve kararlılık kavramına geçeceğiz.

---

## Bugünün tek sorusu

Bir ekonomide:

$$
K_t=200,\quad \delta=0.05,\quad J_t=20
$$

### Semboller / Lejant

- $K_t$: Mevcut sermaye stoku.
- $\delta$: Amortisman oranı.
- $J_t$: Yeni yatırım.
- $K_{t+1}$: Gelecek dönem sermaye stoku.

Şu formülü kullanarak:

$$
K_{t+1}=(1-\delta)K_t+J_t
$$

$K_{t+1}$ değerini hesapla.
