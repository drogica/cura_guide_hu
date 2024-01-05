# Kúpos támasztó minimális szélesség

Ha a kúpos támasz engedélyezve van, és a tartószerkezet zsugorítására van beállítva, ez a beállítás határozza meg azt a minimális szélességet, amelyre a kúpos támasz zsugorítja a tartót. A támaszték nem lesz vékonyabb, hacsak nem vékonyabb a támasztásra szoruló túlnyúlás.

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
"image_path": "support_conical_min_width_20.png",
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
    "support_conical_angle": 30,
    "support_conical_min_width": 15
},
"colours": 64
}-->

![Minimális szélesség 5 mm](../images/support_conical_enabled.png)![Minimális szélesség 15 mm](../images/support_conical_min_width_20.png)

Ha nagy mennyiségű támasz nyugszik egy apró tartóoszlopon, ez a támasz nagyon hajlamos lesz a felborulásra. A minimális szélesség növelése megnöveli annak az alaposzlopnak a szélességét, amelyre a kúp gravitációra fog húzódni. Ez növeli a nyomat megbízhatóságát, de többletanyagba kerül. Összességében a kúpos támaszték kevésbé hatékonyan csökkenti a nyomtatási időt.
