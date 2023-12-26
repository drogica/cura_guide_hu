# Extra kitöltő falszám

Ez a beállítás számos kontúrt ad hozzá a kitöltési területek körül. Ez hasonló a [falak számának](../shell/wall_line_count.md) növeléséhez, de a kontúrok nem keringenek a bőr körül, és a falak a bőr és a kitöltés között is lesznek. Hasonló [a bőr további falainak](../top_bottom/skin_outline_count.md) hozzáadásához is, de nem a bőr körül, hanem a kitöltés körül.

Ezek a falak a kitöltési beállításokkal vannak kinyomtatva.

<!--screenshot {
"image_path": "infill_wall_line_count.png",
"models": [{"script": "hexasphericon.scad"}],
"camera_position": [0, 40, 136],
"settings": {
    "infill_wall_line_count": 2,
    "skin_outline_count": 0
},
"layer": 546,
"colours": 64
}-->

![Két extra fal a kitöltés körül](../images/infill_wall_line_count.png)

A bőr körüli extra falak hozzáadásához képest ez a beállítás nagymértékben növeli a modell szilárdságát és csökkenti a bőrön keresztüli kitöltés láthatóságát, de növeli a nyomtatási időt és az anyagfelhasználást is. Míg az extra bőrfalak helyettesítik azokat az anyagokat, amelyek egyébként is bőrként lettek volna nyomtatva, ez a beállítás valójában anyagot ad hozzá, kivéve, ha a kitöltési sűrűség már 100%.

Ez nagyon hasonló ahhoz, hogy az egész nyomat körül további falakat helyezzenek el. Mindazonáltal célszerű legalább egy extra falat beépíteni akár a kitöltés, akár a bőr köré, mert ez megakadályozza, hogy a bőrvonalak a levegőben végződjenek.
