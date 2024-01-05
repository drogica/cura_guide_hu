# Kúpos alátámasztási szög

Ez a beállítás határozza meg a lejtős szöget, amelynél a kúpos támasz nyomtatásra kerül.

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
"image_path": "support_conical_angle_10.png",
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
    "support_conical_angle": 10
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

![30 fokos szög](../images/support_conical_enabled.png)![10 fokos szög](../images/support_conical_angle_10.png)![-10 fokos szög, aminek következtében az alap szélesebb](../images/support_conical_angle_neg10.png)

A kúpos alátámasztási szög a legnagyobb kompromisszum a támasz stabilitása és a keletkezett alátámasztás között.

Nagy szögben a támaszték nagyon vékony lesz a magasságának nagy részén. Ezzel sok segédanyagot és nyomtatási időt takaríthatunk meg. Ha sok támasztóanyagra van szükség, ez sok időt és anyagot takaríthat meg, mivel a támaszték fele kimarad. Mivel azonban a tartó alul nagyon vékony lesz, a támaszték kevésbé stabillá válhat, ami növeli a nyomat meghibásodásának esélyét. Ennek elkerülése érdekében növelheti a [minimális szélességet](support_conical_min_width.md) .

A negatív szög használatával a támaszték szélesebbé válik az alja felé, vulkán alakúra. Ha a nyomatnak apró részei vannak a magasban, amelyeket alá kell támasztani, akkor általában nagyon magas [tornyok](support_use_towers.md) keletkeznek, amelyek hajlamosak a nyomtatás során felborulni. Negatív szöggel ezek a magas, vékony tartószerkezetek alul szélesebbé válnak. Ez további stabilitást ad nekik. Ennek a támogatásnak a kinyomtatása azonban tovább tart, mivel több anyagot igényel. A körülbelül -5°-os szög általában elegendő ahhoz, hogy még a legmagasabb, legvékonyabb tartószerkezetek is kellő stabilitást biztosítsanak. Ha az anyaga nagyon kiszivárog az utazás során, nagyobb negatív szögre lesz szükség, mert a szerkezet jobban megnyomódik a tartón lévő foltok miatt.
