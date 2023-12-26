# Kitöltés támogatása

Ha engedélyezve van, a kitöltést támogatásként kezeli. Ekkor a kitöltés csak ott jön létre, ahol a felső felület alátámasztásához szükséges. Úgy viselkedik, mintha a modell üreges lenne, és támogatást generál benne, de ez a támogatás a kitöltési beállítások segítségével jön létre.

<!--screenshot {
"image_path": "infill_support_enabled_disabled.png",
"models": [{"script": "stamp.scad"}],
"camera_position": [0, 200, 30],
"settings": {
    "wall_line_count": 0,
    "infill_support_enabled": false
},
"colours": 64
}-->

<!--screenshot {
"image_path": "infill_support_angle_low.png",
"models": [{"script": "stamp.scad"}],
"camera_position": [0, 200, 30],
"settings": {
    "wall_line_count": 0,
    "infill_support_enabled": true,
    "infill_support_angle": 40
},
"colours": 64
}-->

![Normál kitöltés](../images/infill_support_enabled_disabled.png)![Kitöltés támogatása engedélyezve](../images/infill_support_angle_low.png)

- Ez sok anyagot takarít meg a kitöltésnél, nagyon alacsony vizuális költséggel.
- A felső felületek kissé jobban megereszkedhetnek, ha ez engedélyezve van.
- A kitöltés vízszintes szilárdsága azonban csökkenhet. Sok esetben nem lesz kitöltés a falak mögött, ha a falak meredek lejtő részei.
