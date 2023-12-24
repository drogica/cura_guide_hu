# Bridge Skin Flow

Ez a beállítás beállítja az áthidaló alsó oldalak nyomtatásához extrudált anyag mennyiségét.

<!--screenshot {
"image_path": "bridge_skin_density_100.png",
"models": [{"script": "bridge.scad"}],
"layer": 80,
"settings": {
    "bridge_settings_enabled": true,
    "bridge_skin_density": 100,
    "bridge_skin_material_flow": 100,
    "bridge_wall_material_flow": 100
},
"camera_position": [0, 18, 79],
"colours": 64
}-->

<!--screenshot {
"image_path": "bridge_skin_material_flow_50.png",
"models": [{"script": "bridge.scad"}],
"layer": 80,
"settings": {
    "bridge_settings_enabled": true,
    "bridge_skin_density": 100,
    "bridge_skin_material_flow": 50,
    "bridge_wall_material_flow": 100
},
"camera_position": [0, 18, 79],
"colours": 64
}-->

![100%-os áramlásnál a vonalak a normál vonalszélességükben húzódnak](../images/bridge_skin_density_100.png)![50%-os áramlásnál a vonalak vékonyabbak lesznek](../images/bridge_skin_material_flow_50.png)

Az anyagmennyiség csökkentése hatékonyan csökkenti a rést áthidaló alsó oldal vonalszélességét. Csökkentett vonalszélességgel nagyobb a vonalak felület-tömeg aránya, ami lehetővé teszi, hogy gyorsabban lehűljenek, és ez megakadályozza, hogy annyira megereszkedjenek.

Az áramlási sebesség túlzott csökkentése azonban nagy változást fog okozni az áramlási sebességben, különösen, ha [lassabb nyomtatási sebességgel](bridge_skin_speed.md) párosul. A valóságban az anyag nem tudja nagyon gyorsan megváltoztatni az áramlási sebességét, ami miatt a vezetékek a tervezettnél valamivel vastagabbak lesznek az áramlási sebesség lelassulásával, és valamivel vékonyabbak a tervezettnél, ahogy az áramlási sebesség felgyorsul.
