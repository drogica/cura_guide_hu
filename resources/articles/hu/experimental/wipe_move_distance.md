# Törölje a mozgási távolságot

Ezzel a beállítással meghatározhatja, hogy milyen szélesek legyenek a törlőmozgások. A fúvóka ezt a távolságot mozgatja [minden törlési mozdulatnál](wipe_repeat_count.md) .

Kezdetben a fúvóka közvetlenül a törlőkefe mögé kerül egy [bizonyos X koordinátában](wipe_brush_pos_x.md) . Az ennél a beállításnál jelzett távolságnak olyannak kell lennie, hogy ezt a távolságot elmozdítva az ecset másik oldalára kerüljön. A túl messzire való mozgás szükségtelen mozgásokat eredményez, és a fúvóka visszamozdulását okozhatja az építési térfogatba, ami szükségtelenül megütheti a modellt, ha [a Z ugrás nincs engedélyezve](wipe_hop_enable.md) . Ha nem elég messzire mozgatja, megakadályozhatja, hogy megfelelően nekiütődjön a kefének.

A távolság negatív is lehet. Ekkor a fúvóka a másik irányba törli. [Az X koordináta](wipe_brush_pos_x.md) választásától függően ez szükséges lehet a megfelelő irányú törléshez.
