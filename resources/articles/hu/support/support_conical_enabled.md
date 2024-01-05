# Engedélyezze a kúpos támogatást

Ha ez a beállítás engedélyezve van, a tartószerkezet már nem lesz teljesen függőleges az oldalakon. A támasz kúpos alakot kap, az alja felé kisebb vagy nagyobb lesz.

<!--screenshot {
"image_path": "support_conical_enabled.png",
"models": [
    {
        "script": "wide_overhang.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [91, -95, 19],
"settings": {
    "support_enable": true,
    "support_conical_enabled": true,
    "support_conical_angle": 30
},
"colours": 64
}-->

<!--screenshot {
"image_path": "support_conical_angle_neg10.png",
"models": [
    {
        "script": "wide_overhang.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [91, -95, 19],
"settings": {
    "support_enable": true,
    "support_conical_enabled": true,
    "support_conical_angle": -10
},
"colours": 64
}-->

![A támaszték az alja felé csökken](../images/support_conical_enabled.png)![A támaszték az alja felé nagyobb lesz](../images/support_conical_angle_neg10.png)

Maga a támasz egy bizonyos [szögben](support_conical_angle.md) lejt. Negatív szögek esetén a támaszték nagyobb lesz az alsó felé, így a támaszték jelentősen stabilabb lesz. Pozitív szögek esetén az alja felé kisebb lesz. Ezzel rengeteg anyagot és nyomtatási időt takaríthatunk meg. A támaszték instabillá válásának elkerülése érdekében a támasztékhoz [minimális szélesség](support_conical_min_width.md) is meghatározható.

A kúpos alátámasztás a legerősebb paraméter a nyomtatási idő és a támasz stabilitása közötti mérlegelés szempontjából. A kúpos támasztéknak két fő felhasználási esete van:

- Anyag- és nyomtatási idő megtakarítása érdekében. A kúpos alátámasztással könnyedén megspórolhatja a támasztáshoz szükséges anyag felét, és ezzel együtt a nyomtatásra fordított idő felét is. Ez különösen akkor hatékony, ha nagy mennyiségű támogatás van, nagy és magas nyomatokhoz.
- A támasz stabilabbá tétele negatív szög használatával. Ha a nyomatának apró részei vannak a magasban, amelyeket alá kell támasztani, akkor általában nagyon magas [tornyok](support_use_towers.md) keletkeznek, amelyek hajlamosak a nyomtatás során felborulni. Kúpos alátámasztással ezek a magas, vékony tartószerkezetek alul szélesebbé tehetők. Ez további stabilitást ad nekik. Ennek a támogatásnak a kinyomtatása azonban tovább tart, mivel több anyagot igényel.

Ha a [támaszték elhelyezése](support_type.md) úgy van beállítva, hogy csak az építőlemezen helyezze el a támaszt, a kúpos támasz lehetővé teszi, hogy a modell körül nyúljon, hogy továbbra is támassza a modellt olyan helyeken, amelyek a modell többi része felett vannak. A támasz továbbra is csak az építőlemezen fog nyugodni, de formája miatt immár elérheti a kinyúló területeket olyan sarkokban, amelyek egyébként nem lennének alátámasztva.

Ez a funkció valamivel egyszerűbb és kevésbé extrém változata<!-- ha cura_version &gt;= 4.7 --> [Fa támogatás](support_structure.md)<!-- endif --><!-- if cura_version &lt; 4.7:[Tree Support](../experimental/support_tree_enable.md) --> . A fatámasz számos előnnyel rendelkezik, mint a kúpos támaszték. A Tree Support azonban egy teljesen más algoritmust használ, és nagyobb szabadságot kap a támasz felépítésében, míg a kúpos támasz hűbb marad a szokásos támogatásgeneráló algoritmushoz. Ez azt jelenti, hogy a normál támaszték beállításai általában jobban működnek, ha kúpos támasztékkal használják, de jelentősen módosítani kell a fa alátámasztásához. A fa támogatása általában több anyagot és nyomtatási időt takarít meg, miközben megőrzi a nyomtatási megbízhatóságot.
