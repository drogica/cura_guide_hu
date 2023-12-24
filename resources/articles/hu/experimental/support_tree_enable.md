# Fa támogatás

A fa alátámasztás alternatív megközelítést kínál a modell támogatására, mint a hagyományos támogatási technika. A fa alátámasztásánál egy elágazó szerkezet jön létre, amely az építőlemezen kezdődik kis alappal, de a megtámasztást igénylő részek felé nő.

<!--screenshot {
"image_path": "support_structure_tree.png",
"models": [{"script": "duct.scad"}],
"camera_position": [56, 127, 60],
"settings": {
    "support_enable": true,
    "support_structure": "tree",
    "support_tree_collision_resolution": 0.05
},
"colours": 32
}-->

![Egy faszerű szerkezet támasztja alá a túlnyúlást](../images/support_structure_tree.png)

A fa alátámasztása elkerülheti az akadályokat, amikor a túlnyúló területek felé nő. Ha lehetséges, a fát az építőlemeztől felfelé neveljük, hogy elkerüljük a támasztófelület hegesedését. Ha ez nem lehetséges, a fa a modell felületén nyugszik a lehető legközelebb a túlnyúláshoz, hogy minimalizálja az idő- és anyagfelhasználást. A fatartó ágait a [fatámasztó ág szöge](../support/support_tree_angle.md) korlátozza, hogy ne hozzon létre túl meredek túlnyúlást. Ez korlátozza az akadályok körüli növekedését, és meghatározza azt a magasságot is, amelynél a törzsek elkezdenek kiágazni.

A fatámasz alapértelmezés szerint üreges. A fa ágai által körülhatárolt területre azonban továbbra is a szokásos támogatási beállítások érvényesek. Különösen a [Tartósűrűség](../support/support_infill_rate.md) használható arra, hogy a tartószerkezet nagyobb szerkezeti szilárdságot biztosítson. A fa alátámasztásának jellegéből adódóan erősen szaggatott, általában bőven elég ereje van a célnak.

A fa alátámasztás számos előnnyel rendelkezik a normál támogatáshoz képest, hogy néhányat említsünk:

- A fa alátámasztás általában sokkal kevesebb anyagot használ fel, mint a hagyományos támaszték. Az anyagfelhasználás 25-50%-a jellemző. Ezzel sok időt és anyagköltséget takaríthatunk meg.
- Ha ugyanabból az anyagból nyomtatják, mint a nyomatot, a túlnyúlás általában jobban néz ki fa alátámasztás esetén.
- A fatámasz könnyebben eltávolítható, mint a normál támasz.
- A fa alátámasztás kevesebb heget hagy a felületen, mint a normál támaszték, mivel képes a modell körül nyúlni az építőlemez felé.

Ennek azonban vannak hátrányai is:

- A fa alátámasztás nagyságrenddel tovább tart a szeleteléshez. Türelemre lesz szükség, különösen a magas modelleknél.
- A legkisebb ágak kinyomtatása során sok megszakítás történik az áramlásban, így a fatartó nem alkalmas nehezen extrudálható anyagok, például PVA vagy rugalmas anyagok felhasználásával történő nyomtatásra.
- A fatámasz nem működik jól egyes mechanikus modellek támogatásához. Különösen hajlamos arra, hogy túl kevés ágat helyezzen el a lapos, lejtős túlnyúlások megtámasztásához.

Míg a fatámaszt a közönséges támogatással egyidejűleg is lehet aktiválni, ez általában nem kívánatos. A két támasztótípus metszi egymást, és túlextrudálást okoz.
