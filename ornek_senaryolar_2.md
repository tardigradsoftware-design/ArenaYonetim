# Örnek Senaryolar — Seri 2 (Fayda Önce) · Detaylı Görsel Promptları

Sürüm: `v2` · 3 video · 1 ev · 1 bakım · 1 mutfak
Bağlayıcı standart: `ICERIK_KURALLARI.md`

---

## Kaydırma Yasağı Protokolü (no-drift)

Görsel, ses ve yazı **aynı anda aynı şeyi** göstermek zorunda. Ses bir nesneyi
söylüyorsa o nesne karede olmalı. Olmayan nesne kareye girmemeli.

### Kurallar

1. **Adı geçen = karede olan.** Her sahnenin `ZORUNLU NESNELER` listesi vardır.
   Listede olan her nesne karede görünür, görünmüyorsa kare reddedilir.
2. **İkame yasak.** Karbonat yerine un/tuz/şeker, sirke yerine yağ/su, poşet
   yerine kap, lastik yerine ip, diş fırçası yerine sünger çizilmez.
   Renk ve doku da ikame sayılır: sirke **berrak**, karbonat **beyaz toz**.
3. **Fazla nesne de kaydırmadır.** Sesin söylemediği ürün, alet, yiyecek kareye
   girmez. Arka plan yalnızca aynı mekânın sabit dekoru olabilir (tezgâh, fayans,
   ahşap zemin) ve her sahnede aynı kalır.
4. **Durum tutarlılığı.** Kirli → temiz geçişi aynı açıdan, aynı yüzeyde gösterilir.
   Kireç S01'de görünür, S05'te yok. Arada başka bir başlık kullanılmaz.
5. **Olumsuz uyarı sahnelenmez.** "Mermere değdirmeyin" gibi cümlelerde yasak
   kombinasyon **görüntülenmez** (mermer üstünde sirke çekilmez); o sırada izinli
   malzeme gösterilir. Bu, kuralın tek istisnasıdır ve bilerek yapılır.
6. **Yazı ve logo yok.** Ürün etiketleri, rakam, marka, altyazı görselin içinde olmaz.
   Okunabilir tek yazı sonradan eklenen altyazıdır.
7. **İnsan.** Yüz ve gövde yok; yalnızca eller ve bilek. El anatomisi doğru
   (5 parmak, doğru eklem yönü). Hatalı kare teslim edilmez.

### Ortak teknik standart (tüm promptlara eklenir)

Dikey 9:16 · fotogerçekçi · doğal ışık, tek yönlü (sol üstten) · sıcak-nötr renk
paleti · sığ alan derinliği (f/2.8 eşdeğeri), konu net, arka plan hafif bulanık ·
gimbal hizası, hafif göz hizası üstü açı · yüksek detay, doku görünür (gözenek,
kireç, kumaş tüyü) · gürültüsüz, HDR değil.

---

## ORN_V004 — [Ev] Duş Başlığındaki Kireç

**Kanca:** Su azaldıysa suçlu tesisat değil.
**Sahne:** 5 · **Süre:** ~29 sn · **Döngü:** S05 sprey → S01 zayıf sprey

### Seslendirilecek metin (aynen)

> Duşta su azaldıysa ilk bakacağın yer tesisat değil. Başlığın deliklerini kireç tıkıyor ve suyun yarısı boşa gidiyor. Başlığı sök; yarım bardak beyaz sirkeyi yarım bardak suyla karıştır. Başlığı poşete daldırıp ağzını lastikle bağla, otuz dakika bekle. Kireç kalınsa bir saate çıkar. Eski diş fırçasıyla delikleri temizle, tak ve bir dakika soğuk su akıt. Akış açılınca farkı görürsün. Bu yöntem krom ve plastik başlık için; mermer ve doğal taşa sirke değdirmeyin. Bunu kaydet, bir dahaki su azalmasında tekrar izle. Ve unutma...

**Ses dosyası:** `ORN_V004_ses.wav` (yoksa `.mp3`)

### Ses promptu

Sıcak, sakin kadın ses; nötr Türkçe. İlk cümlede hafif şaşkınlık, ölçülerde netlik.
"Yarım bardak", "otuz dakika", "bir saat", "bir dakika" ifadelerinde kısa vurgu ve
200 ms duraklama. Uyarı cümlesi daha yavaş ve ciddi. CTA'da hafif yavaşlama.
Son söz "Ve unutma..." yarım, devamı varmış hissiyle; kesilmez.

### Sahne haritası

| # | Dosya | Ses cümlesi (bu sahnede) | ZORUNLU NESNELER |
|---|---|---|---|
| 1 | `ORN_V004_S01.png` | "Duşta su azaldıysa... deliklerini kireç tıkıyor" | Krom duş başlığı · deliklerde beyaz kireç · zayıf/dağınık su |
| 2 | `ORN_V004_S02.png` | "Başlığı sök; yarım bardak beyaz sirkeyi..." | El · sökülmüş başlık · **iki cam bardak** (biri berrak sirke, biri su) |
| 3 | `ORN_V004_S03.png` | "Başlığı poşete daldırıp ağzını lastikle bağla" | **Şeffaf poşet** · sirke-su · **lastik** · boru |
| 4 | `ORN_V004_S04.png` | "Eski diş fırçasıyla delikleri temizle" | **Eskimiş diş fırçası** · temizlenen delikler · su damlaları |
| 5 | `ORN_V004_S05.png` | "Akış açılınca farkı görürsün... tak ve bir dakika soğuk su akıt" | Takılmış krom başlık · **güçlü ve eşit su** |

### Promptlar (EN — aynen kullan)

**1. `ORN_V004_S01.png`**
```
Vertical 9:16 photorealistic macro shot, extreme close-up of a chrome shower head mounted on a white tiled shower wall, every nozzle ringed with thick chalky white limescale crust, weak uneven water streams falling irregularly with large gaps, a few droplets hanging on the chrome, single soft light from the upper left, shallow depth of field, crisp scale texture, muted warm-neutral palette, no people, no faces, no hands, no text, no logos, no brand marks.
```
ZORUNLU: krom başlık · beyaz kireç halkaları · zayıf/dağınık su · beyaz fayans
YASAK: temiz/parlak başlık · güçlü su · duş teknesi manzarası · şişe/ürün

**2. `ORN_V004_S02.png`**
```
Vertical 9:16 photorealistic image, only two hands and forearms visible unscrewing a detached chrome shower head over a white ceramic bathroom sink, on the counter two clear cylindrical drinking glasses stand side by side and both are filled halfway: the left glass holds clear white vinegar with faint bubbles, the right glass holds plain water, a dry folded grey cloth beside them, soft single-source light from upper left, shallow depth of field, realistic skin texture and nails, warm-neutral palette, no face, no head, no torso, no text, no labels, no packaging.
```
ZORUNLU: iki el · sökülmüş krom başlık · **iki berrak cam bardak** yarım dolu · beyaz lavabo
YASAK: yağ/şişe/etiket · üçüncü bardak · başka alet · kirli tezgâh

**3. `ORN_V004_S03.png`**
```
Vertical 9:16 photorealistic image, a chrome shower head fully submerged inside a clear transparent plastic bag hanging from the shower pipe, the bag contains a clear vinegar-and-water solution reaching halfway up the head, the bag opening is gathered tightly and sealed with a thick tan rubber band around the metal pipe, condensation droplets and slight plastic wrinkles catching the light, white tiled bathroom background softly blurred, single soft light from upper left, shallow depth of field, warm-neutral palette, no people, no hands, no faces, no text, no logos.
```
ZORUNLU: **şeffaf poşet** · içinde sirke-su · **lastik** · asılı başlık · beyaz fayans
YASAK: kova/kase · ip/klips · opak poşet · süre/rakam/saat

**4. `ORN_V004_S04.png`**
```
Vertical 9:16 photorealistic macro image, only one hand holding a worn old toothbrush with splayed splayed bristles, the bristles are scrubbing the nozzle holes of a detached chrome shower head held under running water in a white sink, tiny white scale flakes lifting off the nozzles, clear water sheeting over the chrome, wet metal reflections, single soft light from upper left, shallow depth of field, warm-neutral palette, no face, no torso, no text, no labels, no packaging, no sponge, no brush other than the toothbrush.
```
ZORUNLU: **eskimiş diş fırçası** (dağılmış kıl) · krom başlık delikleri · akan su · kireç döküntüsü
YASAK: sünger · tel fırça · eldiven · yeni/parlak fırça · ürün ambalajı

**5. `ORN_V004_S05.png`**
```
Vertical 9:16 photorealistic macro shot, the same chrome shower head remounted on the white tiled wall, every nozzle now clear and free of scale, strong even symmetrical water streams fanning out, fine mist and bright water highlights, the chrome is polished and reflective, camera angle identical to the first weak-spray shot, single soft light from upper left, shallow depth of field, muted warm-neutral palette, no people, no faces, no hands, no text, no logos.
```
ZORUNLU: temiz krom başlık · **güçlü eşit su** · S01 ile aynı açı
YASAK: kireç kalıntısı · zayıf akış · farklı başlık modeli · etiket

### Tutarlılık sözleşmesi
Aynı banyo, aynı beyaz fayans dokusu, aynı krom başlık modeli ve aynı ışık yönü.
S01 ve S05 **birebir aynı kamera açısı ve mesafe** olmalı (döngü geçişi).
Kireç S01-S02'de görünür, S04'te azalır, S05'te yok.

### Doğruluk notu
Sirke asittir; mermer, traverten ve doğal taşta kullanılmaz. Boyalı/kaplama yüzeyde
uzun bekletme yapılmaz. Çamaşır suyu ile asla karıştırılmaz. Uyarı cümlesinde
yasak malzeme **sahnelenmez**; o sırada izinli yüzey (krom/plastik) gösterilir.

### Yayın metni
**Başlık:** Duşta Su Azaldıysa İlk Bakacağın Yer Tesisat Değil
**Açıklama:** Kireç duş başlığının deliklerini tıkar. 1 ölçü sirke + 1 ölçü su, 30 dakika. Sadece krom ve plastik başlıkta; mermer ve doğal taşa değdirmeyin. Kaydet.
**Etiketler:** duş başlığı kireç, kireç çözme, sirke ile temizlik, pratik ev bilgisi, su tasarrufu
**Hashtag:** #evtemizliği #pratikbilgiler #kireç #banyodüzeni #kaydetmelik

---

## ORN_V005 — [Bakım] Ayakkabı Kokusu

**Kanca:** O koku ayağının değil, ayakkabının suçu.
**Sahne:** 5 · **Süre:** ~29 sn · **Döngü:** S05 kuru ayak/çorap → S01 kapı önü

### Seslendirilecek metin (aynen)

> Ayakkabını çıkarınca gelen koku ayağının değil, ayakkabının suçu. Nemli ortamda bakteriler çoğalır; koku terden değil, onlardan gelir. Her sabah aynı çifti giyiyorsan nemi ayağına geri veriyorsun. Ayakkabıyı yirmi dört saat dinlendir ve dönüşümlü kullan. Akşam içine bir yemek kaşığı karbonat dök, sabah silkele; karbonat nemi çeker. Çorabı pamuklu seç, günde bir kez değiştir ve ayaklarını parmak araları dahil iyice kurula. Koku kaşıntı ve pullanmayla geliyorsa mantar olabilir; kendin çözme, bir uzmana görün. Bunu kaydet, dolabındaki çiftleri ayır. Ve unutma...

**Ses dosyası:** `ORN_V005_ses.wav` (yoksa `.mp3`)

### Ses promptu

Sıcak, sakin kadın ses; nötr Türkçe. İlk cümlede hafif gülümseme, suçlamayan ton.
"Yirmi dört saat", "bir yemek kaşığı", "günde bir kez" ölçülerinde net vurgu.
Mantar uyarısı yavaş ve ciddi. CTA'da hafif yavaşlama. Son söz yarım bırakılır.

### Sahne haritası

| # | Dosya | Ses cümlesi (bu sahnede) | ZORUNLU NESNELER |
|---|---|---|---|
| 1 | `ORN_V005_S01.png` | "Ayakkabını çıkarınca gelen koku..." | **İki çift ayakkabı** · kapı önü · ahşap zemin |
| 2 | `ORN_V005_S02.png` | "...nemli ortamda bakteriler çoğalır" | Tek ayakkabının içi · **nemli, koyulaşmış taban astarı** |
| 3 | `ORN_V005_S03.png` | "Ayakkabıyı yirmi dört saat dinlendir ve dönüşümlü kullan" | **İki çift ayakkabı** · ayakkabı rafı · **bir gözü boş** |
| 4 | `ORN_V005_S04.png` | "Akşam içine bir yemek kaşığı karbonat dök" | **Karbonat kâsesi** · **kaşık** · karbonat ayakkabı içinde |
| 5 | `ORN_V005_S05.png` | "Çorabı pamuklu seç... parmak araları dahil iyice kurula" | **Pamuklu çorap** · havlu · **kuru ayak, parmak arası** |

### Promptlar (EN — aynen kullan)

**1. `ORN_V005_S01.png`**
```
Vertical 9:16 photorealistic image, two pairs of plain unbranded casual shoes standing side by side on a light oak wooden floor beside a white entryway door, one pair neatly aligned leather sneakers, the other pair worn canvas shoes with slightly creased fabric, a thin soft shadow under each shoe, morning daylight entering from the left, shallow depth of field, visible wood grain and shoe texture, warm-neutral palette, no people, no feet inside shoes, no faces, no text, no logos, no brand marks.
```
ZORUNLU: **iki çift ayakkabı** · ahşap zemin · kapı · sabah ışığı
YASAK: üçüncü çift · ayakta giyilmiş ayakkabı · askı/raf (bu sahnede) · logo

**2. `ORN_V005_S02.png`**
```
Vertical 9:16 photorealistic macro image, top-down view into the open mouth of a single worn canvas shoe, the insole filling the frame, its fabric visibly damp and darkened in a broad patch under the toes, faint salt-like tide lines at the edges of the damp area, soft crease shadows and lint texture, the shoe resting on light oak wood, single soft light from the left, shallow depth of field, warm-neutral palette, no people, no hands, no text, no labels, no product packaging, no visible insects or mold colonies.
```
ZORUNLU: tek ayakkabı ağzı · **nemli/koyulaşmış astar** · ahşap
YASAK: görünür bakteri/küf çizimi · ayak · sprey şişesi · etiket

**3. `ORN_V005_S03.png`**
```
Vertical 9:16 photorealistic image, a low two-tier wooden shoe rack in a bright hallway, on the top tier one pair of plain canvas shoes sits neatly, the tier beneath it is completely empty with clean visible wood, a second pair of leather sneakers stands on the floor beside the rack, a soft window light from the left casts a long gentle shadow, shallow depth of field, visible wood grain, warm-neutral palette, no people, no text, no logos, no brand marks.
```
ZORUNLU: **iki çift ayakkabı** (biri rafta, biri yerde) · **boş göz** · ahşap raf
YASAK: dolu raf · karbonat/kaşık (bu sahnede) · kutu/ürün · logo

**4. `ORN_V005_S04.png`**
```
Vertical 9:16 photorealistic image, only hands and forearms visible, one hand holds a plain metal teaspoon filled with fine white baking soda powder, the powder is being tipped into the open mouth of a worn canvas shoe resting on light oak wood, a small clear glass bowl of the same white baking soda powder sits beside the shoe, a thin dusting of powder already visible inside the shoe, warm evening light from the left, shallow depth of field, crisp powder grain texture, warm-neutral palette, no face, no torso, no text, no labels, no packaging, no flour, no sugar, no other ingredient.
```
ZORUNLU: **beyaz karbonat tozu** · **metal yemek kaşığı** · karbonat dolu cam kâse · ayakkabı içinde toz
YASAK: un/şeker/tuz görünümü · kutu ambalaj · başka gıda · ikinci ayakkabı

**5. `ORN_V005_S05.png`**
```
Vertical 9:16 photorealistic close-up of two clean completely dry bare feet resting on a white cotton towel on light oak wood, a hand gently parting the toes of one foot so the skin between them is clearly visible and dry, two neatly folded plain cotton socks lying beside on the towel with visible knit ribbing, soft warm daylight from the left, shallow depth of field, realistic skin and cotton fibre texture, warm-neutral palette, no face, no torso, no text, no logos, no brand tags.
```
ZORUNLU: **kuru ayak** · **parmak arası görünür** · pamuklu çorap (dokulu) · havlu
YASAK: ıslak ayak · krem/şişe · marka etiketi · ikinci kişi

### Tutarlılık sözleşmesi
Aynı ahşap zemin, aynı ayakkabı modelleri (S01/S03), aynı sıcak ışık yönü.
S01'de iki çift yan yana, S03'te biri rafta biri yerde — çift sayısı değişmez (2).
S05'te çorap katlı ve pamuklu dokusu görünür olmalı.

### Doğruluk notu
Karbonat nemi çeker, kokunun kaynağını (bakteri) yok etmez. Mantar şüphesinde
uzmana yönlendirme zorunlu. Şeker hastalığında ayak bakımı ayrıca dikkat ister.

### Yayın metni
**Başlık:** Ayakkabı Kokusu Ayağının Değil, Ayakkabının Suçu
**Açıklama:** Koku nemde çoğalan bakterilerden gelir. 24 saat dinlendirme, dönüşümlü kullanım, akşam 1 kaşık karbonat ve pamuklu çorap. Kaşıntı ve pullanma varsa uzmana görün. Kaydet.
**Etiketler:** ayakkabı kokusu, ayak bakımı, karbonat, pratik bilgi, günlük bakım
**Hashtag:** #ayakbakımı #pratikbilgiler #karbonat #kişiselbakım #kaydetmelik

---

## ORN_V006 — [Mutfak] Sarımsak Soyma

**Kanca:** On dakika harcıyorsan yanlış yerde uğraşıyorsun.
**Sahne:** 5 · **Süre:** ~28 sn · **Döngü:** S05 soyulmuş dişler → S01 kabuklu baş

### Seslendirilecek metin (aynen)

> Sarımsak soymak için on dakika harcıyorsan yanlış yerde uğraşıyorsun. Kabuğu tek tek ayırmak yerine hepsini birden dökeceksin. Başları dişlerine ayır, aynı boyda kuru bir kaba koy ve kapağı kapat. On beş saniye sertçe çalkala; kabuklar kendiliğinden ayrılır. Kalan birkaç diş için bıçağın sırtıyla hafifçe bastır, kabuk çıkar. Taze sarımsakta kabuk daha çok yapışır, süreyi yirmi saniyeye çıkarabilirsin; ezik ve çürük dişleri ayır. Kap kuru olmalı, ıslak kapta kabuk kaymaz. Bunu kaydet, bir dahaki yemekte zaman kaybetme. Ve unutma...

**Ses dosyası:** `ORN_V006_ses.wav` (yoksa `.mp3`)

### Ses promptu

Sıcak, sakin kadın ses; nötr Türkçe. İlk cümlede hafif meydan okuma, gülümseme payı.
"On beş saniye" ve "yirmi saniye" ölçülerinde net vurgu, arada kısa duraklama.
Çalkalama cümlesinde tempo hafif artar, sonra normale döner. CTA'da yavaşlama.
Son söz yarım bırakılır.

### Sahne haritası

| # | Dosya | Ses cümlesi (bu sahnede) | ZORUNLU NESNELER |
|---|---|---|---|
| 1 | `ORN_V006_S01.png` | "On dakika harcıyorsan yanlış yerde uğraşıyorsun" | **Bütün sarımsak başı** · ayrılmış dişler · tahta |
| 2 | `ORN_V006_S02.png` | "Başları dişlerine ayır, kuru bir kaba koy ve kapağı kapat" | Eller · **çelik kase** · **kapak** · dişler |
| 3 | `ORN_V006_S03.png` | "On beş saniye sertçe çalkala" | **Kapaklı kase çalkalanıyor** · hareket bulanıklığı |
| 4 | `ORN_V006_S04.png` | "Bıçağın sırtıyla hafifçe bastır" | **Bıçak yüzü yatık** · avuç içiyle baskı · tek diş |
| 5 | `ORN_V006_S05.png` | "Ezlik ve çürük dişleri ayır... kap kuru olmalı" | **Soyulmuş dişler** · **kabuklar ayrı tabakta** · kuru kase |

### Promptlar (EN — aynen kullan)

**1. `ORN_V006_S01.png`**
```
Vertical 9:16 photorealistic macro image, one whole garlic bulb with its papery white and faintly purple skin intact lying on a light wooden cutting board, six separated unpeeled garlic cloves scattered loosely around it, thin flakes of dry skin and a few crumbs on the wood, a small paring knife lying closed off to the side out of focus, bright soft daylight from the upper left, shallow depth of field, crisp papery skin texture, warm-neutral palette, no people, no hands, no text, no labels, no packaging, no onion.
```
ZORUNLU: **bütün sarımsak başı** · **ayrılmış kabuklu dişler** · tahta · kuru kabuk parçaları
YASAK: soğan · soyulmuş diş (bu sahnede) · kase · etiket/ambalaj

**2. `ORN_V006_S02.png`**
```
Vertical 9:16 photorealistic image, only hands and forearms visible, fingers separating the cloves of a garlic bulb above a dry brushed stainless steel bowl, four unpeeled cloves already resting inside the bowl, a matching stainless steel lid lying flat beside it on a light wooden counter, scattered dry garlic skins on the wood, bright soft daylight from upper left, shallow depth of field, visible brushed metal grain and dry papery skin, warm-neutral palette, no face, no torso, no text, no labels, no packaging, no water, no cloth.
```
ZORUNLU: **çelik kase** (kuru) · **eşleşen kapak** · dişler · ahşap tezgâh
YASAK: su/ıslak kase · bez · plastik kap · cam kavanoz · etiket

**3. `ORN_V006_S03.png`**
```
Vertical 9:16 photorealistic image, only hands and forearms visible shaking a lidded brushed stainless steel bowl vigorously just above a light wooden counter, clear motion blur streaking the hands and the bowl edges, dry garlic skins visibly tumbling and separating inside through the small gap at the lid, a few loose skins landing on the wood, bright soft daylight from upper left, shallow depth of field, dynamic but sharp enough to read the bowl and lid, warm-neutral palette, no face, no torso, no text, no labels, no packaging.
```
ZORUNLU: **kapaklı çelik kase** · güçlü hareket bulanıklığı · **kabuklar ayrılıyor**
YASAK: boş kase · cam kap · su · etiket · iki kase

**4. `ORN_V006_S04.png`**
```
Vertical 9:16 photorealistic macro image, only one hand visible, the heel of the palm pressing down on the flat side of a stainless steel paring knife blade that lies horizontally across a single unpeeled garlic clove on a light wooden board, the blade flat and safe with the cutting edge facing away and clearly not touching the fingers, the clove's dry skin splitting and loosening beneath, bright soft daylight from upper left, shallow depth of field, crisp metal and skin texture, warm-neutral palette, no face, no torso, no text, no labels, no packaging, no blade edge toward fingers.
```
ZORUNLU: **bıçak yüzü yatık** · avuç topuğuyla baskı · tek diş · kabuk çatlıyor
YASAK: bıçak kesici yüzü ele dönük · kesme hareketi · doğrama tahtası üzerinde doğranmış diş

**5. `ORN_V006_S05.png`**
```
Vertical 9:16 photorealistic close-up of a dry brushed stainless steel bowl filled with clean peeled garlic cloves, glossy and intact, a small white ceramic dish beside it holding the collected dry papery skins, the bowl and dish resting on a light wooden board with a dry wooden counter behind, faint traces of dry skin dust on the wood, bright soft daylight from upper left, shallow depth of field, crisp peeled clove texture, warm-neutral palette, no people, no hands, no text, no labels, no packaging, no water droplets.
```
ZORUNLU: **soyulmuş dişler** · **kabuklar ayrı tabakta** · kuru çelik kase · tahta
YASAK: su damlası · ıslak kase · ezik/çürük diş · etiket · ikinci tabak fazlalığı

### Tutarlılık sözleşmesi
Aynı açık renk ahşap tahta ve tezgâh, aynı fırçalanmış çelik kase ve kapak, aynı ışık.
S01 bütün baş → S05 soyulmuş dişler; **aynı kamera mesafesi** (döngü geçişi).
Kabuk miktarı S05'te ayrı tabakta birikmiş olmalı.

### Doğruluk notu
Yöntem taze sarımsakta daha az etkilidir; süre yirmi saniyeye çıkarılır veya bıçak
sırtı yöntemine geçilir. Ezik ve çürük dişler ayrılır. Bıçak yalnızca yüzü yatık
şekilde, avuç topuğuyla bastırılarak kullanılır — kesme hareketi gösterilmez.

---

## Teslim kontrol listesi (görsel ajanı için)

- [ ] Her sahnenin `ZORUNLU NESNELER` listesi karede eksiksiz görünüyor
- [ ] `YASAK` listesindeki hiçbir nesne kareye girmemiş
- [ ] Karbonat = beyaz toz; sirke = berrak sıvı; poşet = şeffaf; lastik = kauçuk halka
- [ ] Yazı, rakam, marka, etiket yok
- [ ] Yüz ve gövde yok; eller doğru anatomi
- [ ] S01 ve S05 döngü için aynı açı
- [ ] Dosya adları birebir: `<KEY>_S0N.png`, PNG, kısa kenar ≥ 1080
- [ ] Eksik/hatalı kare varsa yeniden üretilir, başkasıyla doldurulmaz
