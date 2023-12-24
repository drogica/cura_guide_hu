# Réteg magasság

A 3D nyomtató rétegenként teszi le a műanyagot. A rétegmagasság e rétegek vastagsága milliméterben. Ez a legfontosabb tényező mind a végső nyomat vizuális minőségében, mind a nyomtatási időben.

<!--screenshot {
"image_path": "layer_height_0.1.png",
"models": [{"script": "plunger_stop.scad"}],
"camera_position": [25, 100, 50],
"settings": {"layer_height": 0.1},
"colours": 32
}-->

<!--screenshot {
"image_path": "layer_height_0.3.png",
"models": [{"script": "plunger_stop.scad"}],
"camera_position": [25, 100, 50],
"settings": {"layer_height": 0.3},
"colours": 32
}-->

![0,1 mm rétegmagasság](../images/layer_height_0.1.png)![0,3 mm rétegmagasság](../images/layer_height_0.3.png)

A rétegmagasság az egyetlen legfontosabb beállítás, amely befolyásolja az általános minőséget, és fordítva, a nyomtatási időt. Ez csak néhány a hatások közül:

- A vékonyabb rétegek javítják a nyomat vizuális minőségét. Mivel a rétegek vékonyabbak, csökken a lépcsőfokozó hatás a réteg határain. Ezenkívül a rétegek közelebb kerülnek egymáshoz, így a rétegek közötti gyűrődések kisebbek lesznek, ami összességében simább felületet eredményez.
- A vékonyabb rétegek lehetővé teszik a nyomtató számára, hogy több részletet készítsen a nyomat felső és alsó oldalán.
- A vastagabb rétegek hajlamosak egy bizonyos pontig erősebbé tenni a nyomatot. Kevesebb határ lesz a rétegek között, ami általában gyenge pont. A vastagabb rétegek nem nyírnak annyira.
- A vastagabb rétegek csökkentik a nyomtatási időt, mivel a fúvókának nem kell annyi vízszintes mozgást végeznie.

## Rétegmagasság vs. profilok

Sok beállítás a réteg magasságától függ. Mivel a rétegmagasság jelentősen befolyásolja az anyag áramlási sebességét a fúvókán keresztül, a nyomtatási folyamat számos paramétere megváltozik. Ez nagyon összetett. Például a rétegmagasság növelésekor valószínűleg kissé növelnie kell a nyomtatási hőmérsékletet, hogy ellensúlyozza az extra hőveszteséget. A hőmérséklet ezután befolyásolja az anyag likviditását, ami befolyásolja, hogy milyen élesek lesznek a sarkok, milyen hűtés szükséges stb. Mindig bölcs dolog a nyomtató számára elérhető, előre elkészített minőségi profilból kiindulni, amelynek rétegmagassága közel van a kívánthoz.

Egyedi módban kiválaszthatja a kívánt rétegmagasságot, de az előre elkészített profilok is elérhetők különböző rétegmagassággal. Választhat a különböző rétegmagasságokhoz tartozó profilok közül az Ajánlott módban egy csúszka vagy a legördülő widget segítségével az Egyéni módban. Mivel ezek a profilok a rétegmagasságtól függő paramétereket is megváltoztatnak, így valószínűleg jobb minőséget érhet el.

## További megjegyzések

Nagyon alacsony rétegmagasságnál elérheti a Z tengely felbontási határát. Keresse meg nyomtatója Z tengelyének lépésméretét, és győződjön meg arról, hogy a rétegmagasság ennek többszöröse. Ha nem illeszkedik megfelelően, egyes rétegek vastagabbak lesznek, mint mások, ami sávosodást eredményez.

**Vegye figyelembe, hogy a rétegmagasság beállítása nem érvényes a nyomat kezdeti rétegére vagy a tutajrétegekre, amelyeknek saját beállításai vannak a rétegmagasság külön beállításához. Adaptív rétegek használatakor ez a fóliamagasság-beállítás lesz alapvonal, de a tényleges rétegmagasság némileg változhat.**
