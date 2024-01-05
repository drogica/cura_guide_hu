# Támogatási felület engedélyezése

A „támogatási interfész” egy közvetítő struktúra a normál támogatás és a modell között. Ez a struktúra módosíthatja a támogatás és a modell közötti interfész tulajdonságait anélkül, hogy a támogatás nagy részét jelentősen befolyásolná.

<!--screenshot {
"image_path": "support_interface_enable.png",
"models": [{"script": "trash_bin_lid.scad"}],
"camera_position": [93, 188, 87],
"settings": {
    "support_enable": true,
    "support_interface_enable": true
},
"colours": 64
}-->

![A támogatási felület a kék sötétebb árnyalatával látható](../images/support_interface_enable.png)

Alapértelmezés szerint az interfész rétegek sűrűbbek, mint a normál támogatás. Ez jobb túlnyúló felületet ér el anélkül, hogy sok extra anyagra és nyomtatási időre lenne szüksége. A támaszték eltávolítása azonban nehezebb lesz.

A támogatási felület más extruderrel is nyomtatható, mint a támaszték többi része. Egyes nyomtatási támogatást szolgáló anyagok nagyon drágák és lassan nyomtathatók. Így a támasz nagy része továbbra is az olcsóbb vagy gyorsabb anyaggal kerül kinyomtatásra, de az a felület, ahol a hordozóanyag felhasználása megvalósul, a szebb anyaggal.
