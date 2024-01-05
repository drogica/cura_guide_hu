# Támogatási vonal távolság

Ez a beállítás határozza meg a távolságot a támaszmintázat két szomszédos vonala között. A támaszsűrűség beállításának ez a módja intuitívabb lehet, mint az alátámasztás sűrűségének beállítása, mivel közvetlenül beállítja azt a távolságot, amelyet a megtámasztott vonalaknak át kell hidalniuk.

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

![Nagy vonaltávolság](../images/support_infill_rate_low.png)![Kis vonaltávolság](../images/support_infill_rate_high.png)

A támasztóvonalak közötti távolság csökkentésének vannak pozitív és negatív hatásai. Íme néhány hatás, amelyeket mérlegelni kell:

- Ennek a támasznak a tetején fekvő felület kevésbé fog megereszkedni, mert kisebb távolságot kell áthidalnia két támasztóvonal között.
- A támogatás erősebb lesz, javítva a nyomtatás megbízhatóságát.
- A megnövekedett tapadási felület miatt nehezebb eltávolítani a támasztékot.
- A támogatás kinyomtatásához több anyagra lesz szükség.
- A nyomtatás hosszabb ideig tart.
