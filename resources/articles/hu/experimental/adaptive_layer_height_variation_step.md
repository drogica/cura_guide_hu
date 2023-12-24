# Adaptív rétegek variációs lépésmérete

Ha az egyik réteg kívánt rétegvastagsága nagyon eltér egy szomszédos rétegétől, nagy különbségek lesznek a fúvókán keresztüli áramlási sebességben, ami túlextrudálást vagy alulextrudálást okozhat. Ez a beállítás biztosítja, hogy a rétegvastagság különbsége fokozatos változás legyen, ennek megakadályozására. Ezzel a beállítással megadhatja a maximális rétegvastagság változást két szomszédos réteg között.

<!--screenshot {
"image_path": "adaptive_layer_height_variation_step_0_05.png",
"models": [{"script": "barn.scad"}],
"camera_position": [-108, -229, 118],
"settings": {
    "adaptive_layer_height_enabled": true,
    "adaptive_layer_height_variation_step": 0.05,
    "layer_height": 0.2
},
"colour_scheme": "layer_thickness",
"colours": 128
}-->

<!--screenshot {
"image_path": "adaptive_layer_height_enabled.png",
"models": [{"script": "barn.scad"}],
"camera_position": [-108, -229, 118],
"settings": {
    "adaptive_layer_height_enabled": true,
    "layer_height": 0.2
},
"colour_scheme": "layer_thickness",
"colours": 128
}-->

![A nagy lépésméret lehetővé teszi a rétegvastagság nagyon hirtelen változását](../images/adaptive_layer_height_variation_step_0_05.png)![Kis lépésméret esetén a rétegvastagság változtatása szükséges, hogy egyenletesebb legyen](../images/adaptive_layer_height_enabled.png)

Ennek a beállításnak a csökkentése a rétegvastagság fokozatosabb átmenetére kényszeríti. Ennek számos hatása van a nyomtatásra:

- Kisebb rétegvastagságra való áttéréskor kisebb lesz a túlextrudálás, mert a fúvókán való kiáramlásnak van egy kis ideje, hogy alacsonyabb áramlási sebességhez alkalmazkodjon. Ez megakadályozza a foltok kialakulását a felületen.
- Hasonlóképpen kisebb lesz az alulextrudálás, amikor nagyobb rétegvastagságra váltunk, mivel a fúvókán keresztüli kiáramlás fokozatosan nagyobb áramlási sebességre tud igazodni.
- A sávozás kevésbé lesz látható. Annak ellenére, hogy a különböző rétegvastagságú területeknek továbbra is eltérő lesz a textúrája és színe, ezek a területek most távolabb vannak egymástól, ami megnehezíti a láthatóságot.
- Ahol van egy éles szög a modellben, aminek hirtelen vékonyabb rétegekre való átmenetet kellene okoznia, a topográfiai hatás újra megjelenik. Ennek az az oka, hogy a rétegvastagság nem állítható ilyen gyorsan, így sekélyebb felületekre vastagabb rétegeket kell használni.
- Hasonlóképpen, ha a modellben olyan éles szög van, amely hirtelen átmenetet okoz a vastagabb rétegekre, a nyomtató szükségtelenül vékony rétegeket hoz létre, így a nyomtatási időt veszíti el ott, ahol ez nem szükséges.

Az Adaptive Layers algoritmus implementációja miatt a fokozatos áttérés más rétegvastagságra mindig az átmenetet okozó modellben a szög *felett* fog bekövetkezni.
