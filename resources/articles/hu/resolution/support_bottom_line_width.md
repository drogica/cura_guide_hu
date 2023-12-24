# Támasztja a padlóvonal szélességét

Ez a beállítás beállítja a tartó alsó oldalán lévő vonalak szélességét.

<!--screenshot {
"image_path": "support_bottom_line_width.png",
"models": [
    {
        "script": "gutter_lift.scad",
        "transformation": ["mirrorZ", "scale(0.5)"]
    }
],
"camera_position": [-45, 0, 104],
"camera_lookat": [0, 0, 3],
"settings": {
    "support_enable": true,
    "support_bottom_enable": true,
    "support_bottom_line_width": 0.8
},
"layer": 65,
"colours": 64
}-->

![A tartópadló (sötétebb kék) szélesebb vonalakkal van nyomtatva, mint a támaszték többi része](../images/support_bottom_line_width.png)

A vékonyabb vonalak nyomtatása általában csökkenti a tapadást ott, ahol a támasz a modellen fekszik. Ugyanakkor állandóbbá és megbízhatóbbá teszi a tapadást. Általában könnyebben eltávolítható alátámasztást tesz lehetővé, és kevesebb heget hagy a tárgyon. Természetesen a vékonyabb vonalak nyomtatása is több nyomtatási időt vesz igénybe.
