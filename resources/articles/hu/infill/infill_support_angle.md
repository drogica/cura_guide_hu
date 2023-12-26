# Kitöltési túlnyúlási szög

Kitöltési támogatás használatakor ez a beállítás határozza meg a támogatandó felület minimális túlnyúlási szögét. Ez hasonló a szokásos támaszték [túlnyúlási szög](../support/support_angle.md) beállításához.

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

<!--screenshot {
"image_path": "infill_support_angle_high.png",
"models": [{"script": "stamp.scad"}],
"camera_position": [0, 200, 30],
"settings": {
    "wall_line_count": 0,
    "infill_support_enabled": true,
    "infill_support_angle": 60
},
"colours": 64
}-->

![Az alacsony szög nagyobb alátámasztást eredményez](../images/infill_support_angle_low.png)![A nagy szög kevesebb alátámasztást eredményez](../images/infill_support_angle_high.png)

Ennek a szögnek a növelésével a kitöltés kevésbé tartja meg a felső felületet. Ezzel nyomtatási időt és anyagot takaríthat meg, de a felső héj egy kicsit jobban megereszkedik.

- A 0°-os érték normál kitöltésként fog működni. Mindent támogat.
- A 90°-os érték eltávolítja az összes kitöltő anyagot.
