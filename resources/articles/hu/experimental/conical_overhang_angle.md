# Maximális modellszög

Ezzel a beállítással a túlnyúlás szöge (fokban) van konfigurálva, amely úgy készül, hogy [a kinyúlás nyomtatható legyen](conical_overhang_enabled.md) . Ennek a szögnek a növelése nagyobb túlnyúlást tesz lehetővé, így Cura kevésbé módosítja a modellt. Ennek a szögnek a csökkentésével a tárgy már alig nyúlik ki.

<!--screenshot {
"image_path": "conical_overhang_enabled_enabled.png",
"models": [{"script": "castle.scad"}],
"camera_position": [0, 189, 25],
"settings": {
    "conical_overhang_enabled": true,
    "conical_overhang_angle": 50
},
"colours": 8
}-->

<!--screenshot {
"image_path": "conical_overhang_angle_20.png",
"models": [{"script": "castle.scad"}],
"camera_position": [0, 189, 25],
"settings": {
    "conical_overhang_enabled": true,
    "conical_overhang_angle": 20
},
"colours": 8
}-->

![A modell maximális szöge 50°](../images/conical_overhang_enabled_enabled.png)![A modell maximális szöge 20°](../images/conical_overhang_angle_20.png)

90°-os szög esetén a modell olyan marad, mint volt, teljes kinyúlásával együtt. A modell nem változik. A 0°-os szög minden lejtőt teljesen függőlegessé tesz.

Ennek a szögnek a csökkentése csökkenti a modell túlnyúlását. Ez lehetővé teszi a modell jobb nyomtatását. Nem ereszkedik meg annyira, így az alsó oldalak felülete simább lesz. Ugyanakkor a nyomtatott tárgy kevésbé igazodik az eredeti modellhez. Valamivel több időt és anyagot vesz igénybe a nyomtatás.

A szög negatív is lehet. Így az egész nyomat kúpos, széles alappal. Ez érdekes hatásokat eredményezhet, de nincs valódi gyakorlati haszna.
