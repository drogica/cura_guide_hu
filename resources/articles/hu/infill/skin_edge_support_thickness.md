# Bőrél-támasztó vastagság

Homorú formák nyomtatásakor lesz néhány felső bőr, amely valahol a kitöltés felénél véget ér. Ez a beállítás egy extra vonalat ad a kitöltésen keresztül, hogy megtámassza a bőr szélét, így az egy kicsit kevésbé ereszkedik meg.

<!--screenshot {
"image_path": "skin_edge_support_thickness_0.png",
"models": [
    {
        "script": "stamp.scad",
        "transformation": ["scale(0.4)", "translateZ(-2.5)"]
    }
],
"camera_position": [-29, 29, -50],
"settings": {
    "infill_sparse_density": 10,
    "bottom_thickness": 0,
    "skin_edge_support_thickness": 0
},
"colours": 128
}-->

<!--screenshot {
"image_path": "skin_edge_support_thickness.png",
"models": [
    {
        "script": "stamp.scad",
        "transformation": ["scale(0.4)", "translateZ(-2.5)"]
    }
],
"camera_position": [-29, 29, -50],
"settings": {
    "infill_sparse_density": 10,
    "bottom_thickness": 0,
    "skin_edge_support_thickness": 1
},
"colours": 128
}-->

![A bőr szélét nem támogatja jól a kitöltés](../images/skin_edge_support_thickness_0.png)![A bőr széle alatt egy kerületet húznak át a tölteléken](../images/skin_edge_support_thickness.png)

A kitöltés résein áthaladó egyetlen vonal továbbra is megereszkedik, így a vonal több rétegben is megrajzolható a bőr alátámasztásra szoruló széle alatt. Ez a beállítás a bőr széle alatti vonal függőleges vastagságát konfigurálja. Alternatív megoldásként közvetlenül beállíthatja a [rétegek számát](skin_edge_support_layers.md) a bőr széle alatt, ahol ez a vonal megrajzolódik.

Ennek a vastagságnak a növelése általában a következő hatással lesz a nyomtatásra:

- A bőr széle jobban meg lesz támasztva, ami simább felső részhez vezet, mivel a bőr teljesen áthidalhat egyik oldalról a másikra.
- Kicsit tovább tart a nyomtatás, és több anyagot használ fel.

Ha nagy a feltöltési arány, ennek a beállításnak alig lesz hatása a felső felületre, és [túlextrudálást](../troubleshooting/overextrusion.md) okozhat a kitöltésben. Akkor legjobb 0 mm-en hagyni.
