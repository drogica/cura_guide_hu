# Kitöltési vonal szélessége

A húzott kitöltés minden vonalának szélessége. A vonal szélessége eltérhet a fúvóka méretétől egyszerűen a szükségesnél több vagy kevesebb anyag extrudálásával. Ha több anyagot extrudálnak, a műanyag az oldalak felé folyik, vastagabbá téve a vonalat. Ha kevesebb anyagot extrudálnak, az anyag felületi feszültsége hajlamos arra, hogy az anyagot a fúvóka útjának középvonala felé húzza.

<!--screenshot {
"image_path": "infill_line_width.png",
"models": [{"script": "material_calibration.scad"}],
"camera_position": [35, 92, 122],
"settings": {"infill_line_width": 1},
"layer": 111,
"colours": 64
}-->

![A kitöltő vonalak lényegesen szélesebbek, mint a többi](../images/infill_line_width.png)

A kitöltő vonalak szélesítése erősebbé teheti a nyomtatást és csökkentheti a nyomtatási időt is. Ennek túlzott növelése azonban nagy extrudálási ingadozásokat okozhat. Ez alulextrudálást okoz a kitöltés nyomtatásakor, és túlextrudálást, ha a kitöltés utániakat nyomtat, mivel a fúvókán keresztüli áramlás nem tud elég gyorsan beállni.

**A tényleges kitöltési vonalak szélesebbek lehetnek, mint amit ez a beállítás ír, ha módosította a [Kitöltési réteg vastagsága](../infill/infill_sparse_thickness.md) beállítást.**
