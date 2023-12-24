# Használjon adaptív rétegeket

Az Adaptive Layers helyileg beállítja a nyomat rétegvastagságát, hogy optimalizálja a nyomtatási időt és a minőséget a modell felületi jellemzői alapján. A rétegek vékonyabbak lesznek, ahol sekély lejtők vannak, vagy vastagabbra, ahol a falak meredekek. Ennek az a célja, hogy lehetőség szerint gyorsan nyomtasson, de szükség esetén részletesen is nyomtasson.

<!--screenshot {
"image_path": "adaptive_layer_height_enabled.png",
"models": [{"script": "barn.scad"}],
"camera_position": [-108, -229, 118],
"settings": {
    "adaptive_layer_height_enabled": true,
    "layer_height": 0.2
},
"colour_scheme": "layer_thickness",
"colours": 128
}-->

![A ... val](../images/adaptive_layer_height_enabled.png)

A rétegmagasság úgy van beállítva, hogy a rétegek élei közötti vízszintes távolság állandó maradjon. A sekély felületek kis függőleges elmozdulás mellett nagy vízszintes elmozdulást okoznak, így kis függőleges elmozdulás történik, hogy a vízszintes elmozdulás állandó maradjon. Meredek felületeknél kis vízszintes elmozdulás van nagy függőleges elmozdulással, így nagy függőleges elmozdulás történik, hogy a vízszintes elmozdulás állandó maradjon. Így a rétegek topográfiai hatása állandó marad. A két szomszédos réteg közötti maximális távolság a [Küszöb](adaptive_layer_height_threshold.md) beállítás állandó távolságában marad.

Ha a modellnek mind sekély, mind meredek felületei azonos magasságban vannak, akkor a rétegvastagságot a rétegvastagságok közül a kisebbiknek vesszük. Ez néha szükségtelenül kicsinyíti a rétegmagasságot, mert van mellette egy vízszintes felület. Ez látható a fenti képernyőképen, valamint a bal oldali siló magasságának felénél.

Az Adaptive Layers erősen korlátozva van a nyomtatási minőség javítása érdekében. A rétegmagasság nem térhet el egy megadott [Maximális eltérésnél](adaptive_layer_height_variation.md) nagyobb mértékben az eredeti [Rétegmagasság](../resolution/layer_height.md) beállítástól. Két szomszédos réteg között a rétegmagasság különbsége nem lehet nagyobb egy bizonyos [Lépésméretnél](adaptive_layer_height_variation_step.md) . Ez azt eredményezi, hogy a rétegvastagság fokozatosan átalakul, ahelyett, hogy hirtelen félbevágná egyik rétegről a másikra.

Az adaptív rétegek jelentősen csökkenthetik a nyomtatási időt a nyomtatási minőség romlása nélkül, vagy akár a minőség javítása mellett is. A rétegvastagság beállításának hatása óriási. A legtöbb esetben a nyomtatási idő jelentősen lecsökken a vastagabb rétegek használata miatt, ahol a modell függőlegesen áll. A [topográfiai hatás](../troubleshooting/topography.md) is csökken, mivel a rétegek vízszintesen közelebb vannak egymáshoz.

Ez a funkció azonban számos problémát is okozhat.

- A rétegmagasság változtatásával jellemzően más beállításokat is módosítani kell, például a fúvóka hőmérsékletét. Az adaptív rétegek ezeket sem módosítják automatikusan. Ezáltal a nyomtatás nem lesz optimális pl. túlnyúlások esetén, amelyek alacsonyabb nyomtatási hőmérsékleten jobban teljesítenek.
- Ha a réteg magasságát a teljes rétegen megváltoztatjuk egy kis elemhez a réteg egy kis részén, akkor a réteg többi részén látható lesz a sávozás.
- A függőleges távolságok ezzel is akaratlanul beállíthatók. Ez negatív hatással lehet a nyomtatási minőségre. Például a [felső/alsó vastagság](../top_bottom/top_bottom_thickness.md) általában alacsonyabb lesz, mert a Cura a [Felső rétegek](../top_bottom/top_layers.md) beállítást tartja igaznak, és a rétegek vékonyabbak lesznek. Ez párnázást okozhat. Az érintett beállítások, amelyek már nem megfelelőek, a következők:
    - [Felső vastagság](../top_bottom/top_thickness.md)
    - [Alsó vastagság](../top_bottom/bottom_thickness.md)
    - [Maximális bőrszög a terjeszkedéshez](../top_bottom/max_skin_angle_for_expansion.md)
    - [Fokozatos kitöltés lépcsőmagassága](../infill/gradual_infill_step_height.md)
    - [Fokozatos támogatás kitöltési lépés magassága](../support/gradual_support_infill_step_height.md)
    - [Kitöltőréteg vastagsága](../infill/infill_sparse_thickness.md)
    - [Támogassa a kitöltőréteg vastagságát](../support/support_infill_sparse_thickness.md)
    - [Támogassa a Z távolságot](../support/support_z_distance.md)
    - [Tartsa a tető vastagságát](../support/support_roof_height.md)
    - [Támasz padlóvastagság](../support/support_bottom_height.md)
    - [Támasz túlnyúlási szög](../support/support_angle.md)
    - [Támassza meg a lépcsőfokok magasságát](../support/support_bottom_stair_step_height.md)
    - [Torony tetőszög](../support/support_tower_roof_angle.md)
    - [Ooze Shield Angle](../dual/ooze_shield_angle.md)
    - [Maximális modellszög](../experimental/conical_overhang_angle.md)
