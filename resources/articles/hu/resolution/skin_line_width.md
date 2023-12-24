# Felső/alsó vonal szélessége

A húzott felső és alsó vonal minden vonalának szélessége. A vonal szélessége eltérhet a fúvóka méretétől egyszerűen a szükségesnél több vagy kevesebb anyag extrudálásával. Ha több anyagot extrudálnak, a műanyag az oldalak felé folyik, vastagabbá téve a vonalat. Ha kevesebb anyagot extrudálnak, az anyag felületi feszültsége hajlamos arra, hogy az anyagot a fúvóka útjának középvonala felé húzza.

<!--screenshot {
"image_path": "skin_line_width.png",
"models": [
    {
        "script": "flipper_grip.scad",
        "transformation": ["scale(0.6)"]
    }
],
"camera_position": [0, 37, 107],
"settings": {"skin_line_width": 0.8},
"layer": 300,
"colours": 64
}-->

![A bőrvonalak lényegesen szélesebbek, mint a többi](../images/skin_line_width.png)

A bőrvonalak szélesítése egyszerű módja a nyomtatási idő csökkentésének, mivel kevesebb vonalra lesz szükség az objektum felső és alsó oldalának nyomtatásához. Ennek túlzott növelése azonban nagy extrudálási ingadozásokat okozhat. Ez alulextrudálást okoz a bőr nyomtatása során, és túlextrudálást a következő nyomtatásnál, mivel a fúvókán keresztüli áramlás nem tud elég gyorsan beállni. A bőrvonal szélességének növelése növeli a lyukak megjelenésének esélyét is a felületen, ami nem szép, és megakadályozza, hogy vízzáró legyen.

A bőrvonalak szélességének csökkentése általában szebb felső felületet eredményez, de a nyomtatási idő jelentős költséggel jár. Gyakran hatékonyabb, ha más technikát használ, például [vasalást](../top_bottom/ironing_enabled.md) , vagy csak a [felső felszíni bőrvonalakat](../top_bottom/roofing_line_width.md) állítja be.
