# Támogatási sűrűség

Ez a beállítás határozza meg a tartószerkezetek anyaggal való feltöltésének sebességét. Nagy kitöltési arány esetén a támasztóvonalak nagyon közel kerülnek egymáshoz. Alacsony kitöltési arány esetén a vonalakat távolabb helyezik el egymástól.

<!--screenshot {
"image_path": "support_infill_rate_low.png",
"models": [{"script": "spiral_stair.scad"}],
"camera_position": [-95, 18, 116],
"settings": {
    "support_enable": true,
    "support_infill_rate": 10
},
"layer": 256,
"colours": 64
}-->

<!--screenshot {
"image_path": "support_infill_rate_high.png",
"models": [{"script": "spiral_stair.scad"}],
"camera_position": [-95, 18, 116],
"settings": {
    "support_enable": true,
    "support_infill_rate": 20
},
"layer": 256,
"colours": 64
}-->

![Alacsony támasztósűrűség](../images/support_infill_rate_low.png)![Magas támaszsűrűség](../images/support_infill_rate_high.png)

A támogatási sűrűség növelésének vannak pozitív és negatív hatásai. Íme néhány hatás, amelyeket mérlegelni kell:

- Mivel a támasztóvonalak közötti távolság kisebb, a támaszték tetején felfekvő felület kevésbé fog megereszkedni.
- A támogatás erősebb lesz, javítva a nyomtatás megbízhatóságát.
- A megnövekedett tapadási felület miatt nehezebb eltávolítani a támasztékot.
- A támogatás kinyomtatásához több anyagra lesz szükség.
- A nyomtatás tovább tart.
