# Öntőforma

Ahelyett, hogy magát a modellt nyomtatná ki, ez a funkció azt eredményezi, hogy a nyomtató a modell negatívját, egy öntőformát hoz létre, amelybe egy másik anyagot önthet a modell elkészítéséhez. Ez az öntőforma számos speciális tulajdonsággal rendelkezik, amelyek egyaránt használhatóvá teszik az FFF-nyomtatással történő öntést és nyomtathatók. Ez lehetővé teszi a [Rapid Casting](https://en.wikipedia.org/wiki/Rapid_casting) folyamatát.

<!--screenshot {
"image_path": "mold_enabled_shell.png",
"models": [{"script": "stature.scad"}],
"camera_position": [-78, 160, 228],
"layer": -1
}-->

<!--screenshot {
"image_path": "mold_enabled_mould.png",
"models": [{"script": "stature.scad"}],
"camera_position": [-78, 160, 228],
"settings": {
    "mold_enabled": "True"
},
"colours": 32
}-->

![Egy modell, amelyet el szeretne önteni](../images/mold_enabled_shell.png)![A forma ehhez a modellhez](../images/mold_enabled_mould.png)

A Cura formagenerációja pontosan olyan üregeket hoz létre, amilyen alakot szeretne önteni. Ez az üreg körül egy bizonyos szélességű héj jön létre, amely a [Minimális formaszélesség](mold_width.md) beállítással konfigurálható. Az öntőforma felett és alatt egy bizonyos magasságú borítás jön létre, amely a [Formatető magassága](mold_roof_height.md) beállítással konfigurálható. Ez a bőr azonban nem a modell legtetején keletkezik, így oda lehet önteni az öntőanyagot. Nem is a modell legalján jön létre. Az öntés közben az építőlemezen kell tartania.

## Öntőforma tervezése

Cura penészgenerációja nem tökéletes. Egy-két dolog hiányzik. Íme néhány tipp a javításukhoz.

- A Cura nem hoz létre jeleket a modellben lévő összes helyi maximumhoz. Függőleges rudakat kell hozzáadnia a modellhez, ahol szükség van rácsra.
- A Cura nem teszi lehetővé extra anyag öntését arra az esetre, ha az anyag hűlés közben összezsugorodik. Ha erősen zsugorodó anyagot használ, akkor még a modell legmagasabb pontjához is további csapokat kell hozzáadnia.
- Cura formája mindig egy darabban van. Sok formánál ez azt jelenti, hogy a penészt meg kell semmisíteni az eltávolításhoz. A penészgombák különféle módon elpusztíthatók; csak puszta erővel vagy felmelegítéssel, ha a benne lévő anyag ezt lehetővé teszi, vagy olyan anyag felhasználásával, mint a vízben oldódó PVA.
- A Cura nem teszi lehetővé, hogy rudakat vagy huzalokat helyezzenek bele a forma megerősítésére. Ennek lehetővé tételéhez helyezzen be plusz rudakat a modellbe, hogy a Cura üregeket hagyjon nekik, majd helyezze be a rudat vagy a drótot.
- Az öntőformában lévő alávágások figyelmeztetés nélkül keletkeznek. Ha a gipsznek sok alámetszésre van szüksége, akkor szükséged lesz néhány csonkra vagy más csatornákra, hogy az anyag megfelelően befolyjon, és a levegő távozhasson. Ügyeljen arra is, hogy a penészgombát meg kell semmisíteni, hogy a kiöntést a megszilárdulás után eltávolítsa.

## Anyagok a formanyomtatáshoz

Az ideális forma a következő:

- nagyon merev
- ellenáll a magas hőmérsékletnek
- kémiailag inert, hogy ne tapadjon az öntvényanyaghoz
- nem zsugorodó anyagból készült

Ezenkívül néhány formát meg kell semmisíteni ahhoz, hogy a modellt eltávolítsák. Ebből a célból választhat egy rideg anyagot, vagy olyan anyagot, amely vízzel vagy más vegyszerekkel, például PVA-val oldható.

## Önthető anyagok

Sokféle anyagból lehet öntőformát önteni. Egyesek jobban kompatibilisek a 3D-nyomtatott formákkal, mint mások. Íme néhány példa azokra az anyagokra, amelyek működhetnek:

- **Szilikon** . A szilikon nem kötődik a műanyagokhoz, így könnyen eltávolítható. A szilikon is nagyon rugalmas, és ez enyhe a bevágásokkal szemben. Sőt, a szilikonok hőre keményedőek és hőállóak, így fontolóra veheti a forma leolvasztását a megkötés után. A szilikon öntéséhez azonban speciális szerszámokra van szükség. Különösen szüksége lesz egy vákuumkamrára, hogy kiszivattyúzza a gázbuborékokat a szilikonból.
- **Homok** . A homok ipari szabvány valami negatívum készítésére, mivel nagyon hőálló, de nem kell melegíteni az öntéshez. Öntés után betonnal vagy ragasztóval le lehet kötni, hogy ne essen szét. Ezután egy hőállóbb anyagból készíthet egy másik negatívot.
- **Stukkó** . Hasonló a homokhoz, de általában finomabb szemcsékből készül. Ennek az az előnye, hogy a kötés már benne van az anyagban, így nem kell bekötni. Ez azonban törékenyebb végeredményt eredményezhet.
- **Viasz** . Egyedi gyertyák vagy figurák készítéséhez viaszba öntheti a modellt. A viasz alacsony olvadáspontú, így nem olvasztja meg a penészt. Ezenkívül nem kötődik a műanyagokhoz, így könnyebben válik ki a formából. A viasz nagyon képlékeny és könnyen módosítható a formából való kiemelés után. Ha egyedi gyertyát készít ebből, ne felejtsen el behelyezni egy kanócot, mielőtt megszilárdul.
- **Csokoládé** , különleges, személyre szabott finomságként vagy ajándékként. A csokoládé öntéséhez olvasszuk fel az olvadáspontja fölé, majd öntsük a formába, rázzuk kicsit, hogy a légbuborékok kikerüljenek, és azonnal tegyük be a fagyasztóba. A formát akár hideg vízfürdőbe is helyezheti a fagyasztóba, hogy gyorsabban levonja a hőt. Öt perc múlva óvatosan kivesszük a csokoládét a formából.

Az FFF nyomtatás csak hőre lágyuló műanyagokkal működik. A hőre lágyuló műanyagok olyan műanyagok, amelyek magas hőmérsékleten eleve puhává válnak. Ez nem kompatibilis az öntési anyagokkal, amelyek öntés közben forróak. Néhány anyag, amely általában nem kompatibilis a 3D nyomtatott öntőformákkal:

- **Fémek** , amelyeket a műanyagok olvadáspontja fölé kell hevíteni, hogy elég folyékonyak legyenek az öntéshez. A fém hőtömegének hatására a penész megolvad.
- **Műanyagok, amelyek hozzákötődnek** ahhoz a műanyaghoz, amelyből a forma készül. Öntés után nem lehetett elválasztani a formát a modelltől. Szórhatunk bele némi formaleválasztót, de ha az anyag túlságosan hasonló, akkor is tartósan a formához kötődik.
- **Olyan anyagok, amelyek túlságosan zsugorodnak** a megszilárdulás után. Azok az anyagok, amelyek a megszilárdulás előtt zsugorodnak, rendben vannak, ha kellően hosszú szárak vannak ahhoz, hogy új anyag töltse ki az üreget, amikor ez megtörténik.
- **Az epoxigyanta** nem megfelelő, mert míg a gyanta öntés közben hideg, a két komponens kémiai reakciója során elegendő hő szabadul fel a műanyag megolvasztásához. Az epoxi is nagyon jól tapad a műanyagokhoz.

Ha olyan anyagból kell objektumot létrehoznia, amely nem közvetlenül kompatibilis a 3D nyomtatással, akkor több öntési szakaszban kell dolgoznia. Minden szakasz létrehozza az előző szakasz negatívját. Például kinyomtathatja a tárgy alakját a szokásos módon (ez a beállítás ki van kapcsolva), majd létrehozhat egy negatívot úgy, hogy a formát stukkófürdőbe helyezi. Mivel a stukkó sokkal hőállóbb, használhat olyan anyagokat, amelyeket melegebbre kell melegíteni az olvadáshoz, például bronzot, vagy olyan anyagokat, amelyek a műanyagokhoz kötődnek, például az epoxi.

## Az öntés folyamata

A 3D nyomtatott formával történő öntés nagyjából ugyanaz, mint bármely más formánál, és nagymértékben függ a felhasznált anyagoktól. A 3D nyomtatott öntőformák esetében azonban van néhány különös figyelem.

A hőre lágyuló műanyag, amellyel a formáját nyomtatta, alacsony hőkapacitású, és meglehetősen alacsony üvegesedési hőmérséklettel rendelkezik. Ez azt jelenti, hogy a forma öntése után az idő a lényeg. Ha az anyag túl lassan hűl le, a penész megpuhulhat. Ez a forma deformálódását okozhatja, és megnehezíti a forma kioldását az eredményből. A gipsz kötésének felgyorsítása érdekében például jeges fürdőbe márthatja.

A 3D nyomtatott formák oldalain is több bordás van a rétegek közötti határok miatt. Ezek megnehezítik a forma kioldását az öntvényből. Ha elválasztószert használ a forma és az öntvény között, használjon valamit, ami kitölti ezeket a hézagokat. A vékony kenőanyagok nem elegendőek. A megfelelőbb felületi rétegek a viasz vagy a vastagabb kenőanyagok.
