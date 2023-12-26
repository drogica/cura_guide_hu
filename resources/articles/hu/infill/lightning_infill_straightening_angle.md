# Villámfeltöltés kiegyenesítő szög

Ez a beállítás határozza meg, hogy a Lightning kitöltési minta milyen meredeken nyúlhat ki belülről.

A villámkitöltés a névleges villámszerű cikk-cakk vonalakat hozza létre, ahol meg kell támasztani a nyomat tetejét, de ezek nyomtatása hosszú időt vesz igénybe a vonalak éles sarkai miatt. Az alábbiakban tehát megpróbálja kiegyenesíteni a szaggatott vonalakat, hogy csökkentse a nyomtatási időt. Ez az egyengetés túlnyúlásokat okoz. A beállítás határozza meg, hogy mekkora túlnyúlás megengedett.

<!--screenshot {
"image_path": "lightning_infill_straightening_angle_40.png",
"models": [
    {
        "script": "cylinder.scad",
        "transformation": ["scaleZ(0.5)"]
    }
],
"camera_position": [36, 44, 19],
"settings": {
    "infill_pattern": "lightning",
    "wall_line_count": 0,
    "top_layers": 0,
    "lightning_infill_support_angle": 40,
    "lightning_infill_prune_angle": 10,
    "lightning_infill_straightening_angle": 40
},
"colours": 32
}-->

<!--screenshot {
"image_path": "lightning_infill_straightening_angle_10.png",
"models": [
    {
        "script": "cylinder.scad",
        "transformation": ["scaleZ(0.5)"]
    }
],
"camera_position": [36, 44, 19],
"settings": {
    "infill_pattern": "lightning",
    "wall_line_count": 0,
    "top_layers": 0,
    "lightning_infill_support_angle": 40,
    "lightning_infill_prune_angle": 10,
    "lightning_infill_straightening_angle": 10
},
"colours": 32
}-->

![40°-nál a kitöltő vonalak gyorsan egyenes vonalakká konvergálnak](../images/lightning_infill_straightening_angle_40.png)![10°-nál már nincsenek meredek túlnyúlások a kitöltésben](../images/lightning_infill_straightening_angle_10.png)

A gyors kiegyenesítés (megnövelt túlnyúlás) valamelyest csökkenti a nyomtatási időt, de csökkenti a nyomat megbízhatóságát is, különösen vékony vonalszélesség esetén. Ha a túlnyúlás túl meredek, ez réteghasadást eredményez. A hasadás a nyomat belsejében lesz, és gyakran nem okoz problémát, de a kitöltésnek ez a része teljesen meghibásodhat, ami azt eredményezheti, hogy a felső oldal egy része nem támogatott. Ez ezután durva foltként vagy párnázásként lesz látható a tetején, vagy a legrosszabb esetben akár összekeveredett műanyagként.
