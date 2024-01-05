# Támogassa a kitöltési vonal utasításait

A támasztóminta általában úgy van orientálva, hogy a vonalak merőlegesek a legtöbb általa támogatott dologra. Így minimálisra csökken az a távolság, amelyet a megtámasztott anyagnak át kell hidalnia. Ezzel a beállítással a támasztóvonalak tájolása testreszabható.

<!--screenshot {
"image_path": "support_infill_angle_0.png",
"models": [{"script": "umbrella_square_rounded.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "support_enable": true,
    "support_infill_angles": [0]
},
"layer": 160,
"colours": 64
}-->

<!--screenshot {
"image_path": "support_infill_angle_30.png",
"models": [{"script": "umbrella_square_rounded.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "support_enable": true,
    "support_infill_angles": [30]
},
"layer": 160,
"colours": 64
}-->

<!--screenshot {
"image_path": "support_infill_angles.png",
"models": [{"script": "umbrella_square_rounded.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "support_enable": true,
    "support_infill_angles": [30, 60]
},
"layer": 160,
"colours": 64
}-->

![0°-os szög](../images/support_infill_angle_0.png)![30°-os szög](../images/support_infill_angle_30.png)![30° és 60° között váltakozva](../images/support_infill_angles.png)

Ez a beállítás lehetővé teszi több szög megadását, vesszővel elválasztva. Ha több szöget ad meg, a Cura váltogatja ezeket a szögeket a rétegeken.

Ha a [felső/alsó vonal irányait](../top_bottom/skin_angles.md) beállította, célszerű ennek megfelelően beállítani a támasz szögét, hogy az továbbra is merőleges legyen a nyomat alsó oldalának vonalaira. Ez lehetővé teszi, hogy ezek az alsó vonalak megfelelően felfeküdjenek a támasztékra, ahelyett, hogy a támasztóvonalak közé esnének. Ez különösen fontos vonalak és cikkcakkos [támaszmintázatok](support_pattern.md) esetén, ahol hosszú egyenesek vannak a támasztóvonalak között, amelyek nem nyújtanak semmilyen támaszt.
