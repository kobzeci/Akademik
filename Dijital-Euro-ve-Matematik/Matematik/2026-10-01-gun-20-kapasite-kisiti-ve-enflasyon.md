# Gün 20 — Kapasite Kısıtı ve Enflasyon

## Amaçlı Dijital Euro ne zaman reel üretim, ne zaman fiyat baskısı yaratır?

Dün input-output çerçevesinde şu sonuca ulaştık:

$$
VA=\mathbf{v}'(I-A)^{-1}BD_s\mathbf{I}
$$

### Semboller / Lejant

- $VA$: Toplam yurtiçi katma değer.
- $\mathbf{v}$: Sektörel katma değer katsayıları vektörü.
- $I$: Birim matris.
- $A$: Teknik girdi katsayıları matrisi.
- $(I-A)^{-1}$: Leontief tersi.
- $B$: Amaçlı dijital paranın nihai talebe dönüşüm matrisi.
- $D_s$: Sterilizasyon sonrası kalan oranları gösteren matris.
- $\mathbf{I}$: Brüt amaçlı Dijital Euro ihraç vektörü.

Bu formül, talebin üretim ağı boyunca nasıl yayıldığını gösteriyordu. Fakat kritik bir varsayımı sessizce yapıyorduk: ekonomi talep edilen miktarı üretebiliyor.

Bugün bu varsayımı kaldırıyoruz.

Temel soru şu:

> Amaçlı Dijital Euro ile talep yaratıldığında, reel kapasite yeterli değilse ne olur?

Bu soru tezin merkezindeki “parasal genişleme yaratmadan değer üretme” iddiasını test etmek için zorunludur.

---

## 1. Fiilî üretim ile potansiyel üretim

Bir ekonominin fiilî üretimini $Y$, potansiyel üretimini $Y^*$ ile gösterelim.

$$
G=Y^*-Y
$$

### Semboller / Lejant

- $Y$: Fiilî reel üretim.
- $Y^*$: Enflasyonu hızlandırmadan sürdürülebilir kabul edilen potansiyel üretim.
- $G$: Kapasite veya çıktı açığı.
- $^*$: Burada potansiyel/denge düzeyini gösterir.

Örneğin:

$$
Y^*=120
$$

ve:

$$
Y=90
$$

ise:

$$
G=120-90=30
$$

Ekonomide 30 birimlik kullanılabilir üretim alanı vardır.

Bu basitleştirilmiş anlatımda $G>0$ olması boş kapasite bulunduğunu gösterir.

---

## 2. Kapasite kullanım oranı

Aynı bilgiyi oran biçiminde de yazabiliriz:

$$
u=\frac{Y}{Y^*}
$$

### Semboller / Lejant

- $u$: Kapasite kullanım oranı.
- $Y$: Fiilî üretim.
- $Y^*$: Potansiyel üretim.

Örneğin:

$$
u=\frac{90}{120}=0.75
$$

yani kapasite kullanımı yüzde 75'tir.

Boş kapasite oranı:

$$
1-u
$$

olduğuna göre:

$$
1-0.75=0.25
$$

yani yüzde 25'tir.

---

## 3. Amaçlı para talep yaratıyor

Amaçlı Dijital Euro'nun net talep etkisini basitçe:

$$
D=b(1-s)I
$$

şeklinde yazalım.

### Semboller / Lejant

- $D$: Oluşan ilave nihai talep.
- $I$: Brüt amaçlı Dijital Euro ihracı.
- $s$: Sterilizasyon oranı.
- $1-s$: Ekonomide etkili kalan oran.
- $b$: Net paranın harcamaya dönüşme oranı.

Örneğin:

$$
I=100,\quad s=0.20,\quad b=0.75
$$

ise önce net para:

$$
(1-s)I=0.80\times100=80
$$

olur.

Sonra harcamaya dönüşen talep:

$$
D=0.75\times80=60
$$

olur.

Yani 100 birimlik brüt ihraç, bu örnekte 60 birimlik ilave talep oluşturur.

---

## 4. Talep boş kapasiteden küçükse

Basit bir ilk yaklaşım olarak:

$$
D\leq G
$$

ise ilave talebin büyük kısmının reel üretim artışıyla karşılanabileceğini düşünelim.

Örneğin:

$$
G=30
$$

ve:

$$
D=20
$$

ise ekonomi teorik olarak bu ek talebi mevcut boş kapasiteyle karşılayabilir.

Basitleştirilmiş olarak:

$$
\Delta Y=D
$$

yazabiliriz.

### Semboller / Lejant

- $\Delta Y$: Reel üretimdeki değişim.
- $D$: İlave talep.

Bu elbette çok güçlü bir varsayımdır. Gerçek ekonomide işgücü, ara mal, enerji ve ithalat darboğazları nedeniyle tüm talep üretime dönüşmeyebilir. Ama kapasite mantığını öğrenmek için iyi bir başlangıçtır.

---

## 5. Talep kapasite açığını aşarsa

Şimdi:

$$
D>G
$$

olsun.

Örneğin:

$$
G=30
$$

ama:

$$
D=50
$$

olsun.

İlk 30 birim talep boş kapasiteyi kullanabilir.

Geriye:

$$
50-30=20
$$

birim fazla talep kalır.

Buna basitçe aşırı talep diyelim:

$$
E=\max(0,D-G)
$$

### Semboller / Lejant

- $E$: Kapasiteyi aşan fazla talep.
- $\max(0,D-G)$: $D-G$ negatifse sıfır, pozitifse pozitif farkı alır.
- $D$: İlave talep.
- $G$: Kapasite açığı.

Örnekte:

$$
E=\max(0,50-30)=20
$$

olur.

---

## 6. Fazla talebi enflasyona bağlamak

En basit fiyat baskısı denklemini:

$$
\Delta \pi=\phi E
$$

olarak kuralım.

### Semboller / Lejant

- $\Delta\pi$: Enflasyondaki değişim.
- $\phi$: Aşırı talebin fiyatlara geçiş katsayısı.
- $E$: Kapasiteyi aşan talep.

Örneğin:

$$
\phi=0.05
$$

ve:

$$
E=20
$$

ise:

$$
\Delta\pi=0.05\times20=1
$$

olur.

Burada “1”in yüzdelik puan mı başka ölçek mi olduğu modelin kalibrasyonuna bağlıdır. Şimdilik önemli olan yön ve mekanizmadır.

---

## 7. Paranın reel ve fiyat etkisini ayırmak

Şimdi iki parçalı basit sistemimiz var.

Reel üretim etkisi:

$$
\Delta Y=\min(D,G)
$$

Enflasyonist fazla talep:

$$
E=\max(0,D-G)
$$

ve:

$$
\Delta\pi=\phi E
$$

### Semboller / Lejant

- $\min(D,G)$: $D$ ile $G$ arasındaki küçük olan değeri alır.
- $\max(0,D-G)$: Kapasiteyi aşan kısmı seçer.
- $\Delta Y$: Reel üretim artışı.
- $\Delta\pi$: Enflasyon değişimi.

Bu üç denklem çok basit olsa da tezin temel sezgisini güçlü biçimde gösteriyor:

> Aynı para miktarı, ekonominin kapasite durumuna bağlı olarak farklı oranlarda reel üretime veya fiyat artışına dönüşebilir.

---

## 8. Aynı para, iki farklı ekonomi

Amaçlı para 40 birim ilave talep yaratsın:

$$
D=40
$$

### Ekonomi A

$$
G_A=60
$$

olduğunda:

$$
\Delta Y_A=\min(40,60)=40
$$

ve:

$$
E_A=\max(0,40-60)=0
$$

Dolayısıyla:

$$
\Delta\pi_A=0
$$

basitleştirilmiş sonucunu elde ederiz.

### Ekonomi B

$$
G_B=10
$$

ise:

$$
\Delta Y_B=\min(40,10)=10
$$

ve:

$$
E_B=\max(0,40-10)=30
$$

olur.

Aynı para programı ikinci ekonomide çok daha enflasyonisttir.

---

## 9. Sektörel kapasite

Çok katmanlı Dijital Euro için tek toplam kapasite yeterli değildir.

Her sektör için:

$$
G_i=Y_i^*-Y_i
$$

yazabiliriz.

### Semboller / Lejant

- $i$: Sektör indeksi.
- $G_i$: $i$. sektörün kapasite açığı.
- $Y_i^*$: Sektörün potansiyel üretimi.
- $Y_i$: Sektörün fiilî üretimi.

Amaçlı talep de sektörlere göre ayrılır:

$$
D_i
$$

Böylece:

$$
E_i=\max(0,D_i-G_i)
$$

ve:

$$
\Delta\pi_i=\phi_i E_i
$$

yazabiliriz.

---

## 10. Input-output ile kapasite kısıtını birleştirmek

Dünkü modelde:

$$
\mathbf{x}^{req}=(I-A)^{-1}\mathbf{d}
$$

ile talebi karşılamak için gereken üretimi hesaplıyorduk.

### Semboller / Lejant

- $\mathbf{x}^{req}$: Talebi karşılamak için gereken sektörel üretim vektörü.
- $(I-A)^{-1}$: Leontief tersi.
- $\mathbf{d}$: Nihai talep vektörü.

Fiziksel kapasite vektörünü:

$$
\bar{\mathbf{x}}
$$

ile gösterelim.

Gerçekleşebilecek üretim için kaba bir ifade:

$$
x_i^{act}=\min(x_i^{req},\bar x_i)
$$

olabilir.

### Semboller / Lejant

- $x_i^{act}$: Gerçekleşebilen üretim.
- $x_i^{req}$: Talebin gerektirdiği üretim.
- $\bar x_i$: Sektörün azami mevcut üretim kapasitesi.

Talep edilen üretim kapasiteyi aşıyorsa:

$$
g_i=x_i^{req}-\bar x_i>0
$$

bir darboğaz oluşur.

---

## 11. Darboğaz yalnızca o sektörü etkilemeyebilir

Input-output yapısında bir sektör diğer sektörlerin girdisidir.

Bunu sezgisel olarak:

$$
\Delta\boldsymbol{\pi}=F\mathbf{g}
$$

şeklinde yazabiliriz.

### Semboller / Lejant

- $\Delta\boldsymbol{\pi}$: Sektörel fiyat değişimleri vektörü.
- $\mathbf{g}$: Sektörel kapasite aşımı/darboğaz vektörü.
- $F$: Darboğazların sektörler arası fiyatlara yayılmasını gösteren matris.

---

## 12. İthalat kapasite supabı olabilir

Fazla talebin bir oranı ithalatla karşılansın:

$$
M=\mu E
$$

### Semboller / Lejant

- $M$: İlave ithalat.
- $\mu$: Fazla talebin ithalata giden oranı.
- $E$: Kapasiteyi aşan talep.

Kalan iç fiyat baskısı:

$$
E^{dom}=(1-\mu)E
$$

olur.

Ve:

$$
\Delta\pi=\phi(1-\mu)E
$$

yazabiliriz.

Bu kısa vadeli enflasyonu azaltabilir; fakat döviz talebi ve dış denge maliyeti yaratabilir.

---

## 13. Amaç fonksiyonu

Artık bir para programını üç çıktı üzerinden değerlendirebiliriz:

- yurtiçi katma değer $VA$,
- enflasyon etkisi $\Delta\pi$,
- ithalat ihtiyacı $M$.

Basit bir amaç fonksiyonu:

$$
W=VA-\lambda_\pi(\Delta\pi)^2-\lambda_M M
$$

olabilir.

### Semboller / Lejant

- $W$: Politika/refah amaç fonksiyonu.
- $VA$: Yurtiçi katma değer.
- $\lambda_\pi$: Enflasyon maliyetine verilen ağırlık.
- $(\Delta\pi)^2$: Büyük enflasyon sapmalarını giderek daha maliyetli yapan karesel terim.
- $\lambda_M$: İthalat/döviz maliyetine verilen ağırlık.
- $M$: İlave ithalat.

Bu, “enflasyon yaratmadan değer yaratmak” fikrini daha savunulabilir bir araştırma sorusuna dönüştürür.

---

## 14. Sterilizasyonu geri besleme kuralına çevirmek

Sterilizasyon oranını sabit bırakmayalım.

$$
s_t=s_0+\gamma(u_t-u^*)
$$

### Semboller / Lejant

- $s_t$: $t$ dönemindeki sterilizasyon oranı.
- $s_0$: Normal koşullardaki temel sterilizasyon oranı.
- $\gamma$: Sterilizasyon tepkisinin gücü.
- $u_t$: Mevcut kapasite kullanım oranı.
- $u^*$: Referans kapasite kullanım oranı.

Eğer:

$$
u_t>u^*
$$

ise:

$$
s_t>s_0
$$

olur.

Ekonomi kapasite sınırına yaklaşırken sistem otomatik olarak daha fazla likiditeyi geri çeker.

---

## 15. Enflasyonu da geri beslemeye eklemek

Daha ileri bir kural:

$$
s_t=s_0+\gamma_u(u_t-u^*)+\gamma_\pi(\pi_t-\pi^*)
$$

olabilir.

### Semboller / Lejant

- $\gamma_u$: Kapasite sapmasına verilen sterilizasyon tepkisi.
- $\gamma_\pi$: Enflasyon sapmasına verilen sterilizasyon tepkisi.
- $\pi_t$: Mevcut enflasyon.
- $\pi^*$: Hedef/referans enflasyon.

Bu, sabit sterilizasyon yerine duruma bağlı bir para kuralıdır.

---

## 16. Aşırı tepki riski

Eğer $\gamma_u$ veya $\gamma_\pi$ çok yüksek olursa sistem aşırı tepki verebilir:

1. enflasyon biraz yükselir,
2. sterilizasyon sertleşir,
3. talep hızla düşer,
4. üretim kapasitesi boş kalır,
5. sistem yeniden genişler,
6. talep tekrar sıçrar.

Bu, dinamik sistemler ve kontrol teorisinde inceleyeceğimiz salınım ve kararlılık problemidir.

İleride:

$$
x_{t+1}=Ax_t+Bu_t
$$

gibi sistemlere geçeceğiz.

---

## 17. Küçük türetme: enflasyonist bölgeye geçmeden azami ihraç

Net talep:

$$
D=b(1-s)I
$$

olsun.

Kapasiteyi aşmama koşulu:

$$
D\leq G
$$

Yerine koyalım:

$$
b(1-s)I\leq G
$$

$I$ için çözelim:

$$
I\leq\frac{G}{b(1-s)}
$$

Dolayısıyla basit modelde:

$$
I_{\max}=\frac{G}{b(1-s)}
$$

### Semboller / Lejant

- $I_{\max}$: Kapasite sınırını aşmadan yapılabilecek azami brüt ihraç.
- $G$: Mevcut boş kapasite.
- $b$: Paranın talebe dönüşme oranı.
- $s$: Sterilizasyon oranı.

Formülden:

$$
G\uparrow \Rightarrow I_{\max}\uparrow
$$

yani boş kapasite arttıkça daha fazla ihraç alanı vardır.

$$
b\uparrow \Rightarrow I_{\max}\downarrow
$$

çünkü yaratılan para daha hızlı talebe dönüşür.

Sterilizasyon arttığında $1-s$ küçüldüğü için kapasite sınırı açısından daha yüksek brüt ihraç mümkün olabilir; ancak bunun yatırım ve büyüme maliyetini henüz hesaba katmıyoruz.

---

## 18. Tez bağlantısı

Bugünkü çerçeve tezindeki iddiayı daha hassas hale getiriyor.

Aşırı güçlü ifade:

> Amaçlı dijital para enflasyon yaratmadan üretim yaratabilir.

Daha savunulabilir ifade:

> Amaçlı dijital para, kullanılmayan reel kapasiteye, düşük ithalat sızıntısına ve yeterli arz esnekliğine yönlendirildiği ölçüde nominal talebin daha yüksek bölümünü reel üretim ve katma değere çevirebilir; kapasite sınırına yaklaşıldığında fiyat ve dış denge maliyetleri hızlanabilir.

Tezin özgün kısmı daha sonra şu soruya dönebilir:

> Dijital paranın koşullu altyapısı sayesinde para tahsisi ve sterilizasyon oranları sektörlerin anlık kapasite, fiyat ve ithalat durumlarına göre ayarlanabilir mi?

Bu soru bizi doğrudan dinamik kontrol problemine götürüyor.

---

## Bugünün özeti

Talep:

$$
D=b(1-s)I
$$

Kapasite açığı:

$$
G=Y^*-Y
$$

Reel üretime dönüşebilecek bölüm:

$$
\Delta Y=\min(D,G)
$$

Fazla talep:

$$
E=\max(0,D-G)
$$

Enflasyon etkisi:

$$
\Delta\pi=\phi E
$$

ve basit kapasite sınırı:

$$
I_{\max}=\frac{G}{b(1-s)}
$$

olarak yazılabilir.

Bugünün ana dersi:

> Paranın enflasyonist olup olmadığını yalnızca para miktarı değil, paranın karşılaştığı reel kapasite belirler.

Sonraki derste kapasiteyi sabit bir tavan olmaktan çıkarıp yatırım yoluyla potansiyel üretimin zaman içinde nasıl büyüdüğünü kurarak ilk gerçek dinamik denklem sistemimize geçeceğiz.

---

## Bugünün tek sorusu

Bir ekonomide:

$$
Y^*=150
$$

ve:

$$
Y=120
$$

olsun.

### Semboller / Lejant

- $Y^*$: Potansiyel üretim.
- $Y$: Fiilî üretim.
- $G$: Kapasite/çıktı açığı.

Şu formülü kullanarak:

$$
G=Y^*-Y
$$

kapasite açığı $G$'yi hesapla.
