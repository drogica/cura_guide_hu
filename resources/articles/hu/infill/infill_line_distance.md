# Kitöltési vonal távolság

A [kitöltési sűrűség](infill_sparse_density.md) százalékos beállítása helyett lehetőség van a kitöltési sűrűség konfigurálására is a szomszédos kitöltési vonalak közötti távolság beállításával. A kitöltő vonalak közötti nagyobb távolság összességében alacsonyabb feltöltési sűrűséget eredményez.

A kitöltési vonal távolsága másképp nézi ezt a tulajdonságot, mint a sűrűség. A kitöltési vonalak közötti távolság azt a távolságot jelzi, amelyet a felső felületi vonalaknak át kell haladniuk egyik kitöltővonaltól a másikig. A betöltési vonal távolságának csökkentése így csökkenti az áthidalt távolságot és javítja a felső felületek minőségét.

<!--screenshot {
"image_path": "infill_pattern_grid.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "grid"
},
"colours": 64
}-->

<!--screenshot {
"image_path": "infill_sparse_density_low.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_sparse_density": 10
},
"colours": 64
}-->

![4 mm-es távolság a vonalak között, ami 20%-os sűrűséget eredményez](../images/infill_pattern_grid.png)![8 mm-es távolság a vonalak között, ami 10%-os sűrűséget eredményez](../images/infill_sparse_density_low.png)

Általában a kitöltési vonal távolságot a kívánt kitöltési sűrűségből számítják ki, a kiválasztott kitöltési mintától és a vonal szélességétől függően. A kitöltési vonal távolsága vezet.

A kitöltési sűrűség növelése (a vonaltávolság csökkentésével) nagy hatással van a nyomtatásra, nevezetesen:

- A nyomat erősebb lesz.
- A felső felület jobban alátámasztva lesz, így simább és vízzáróbb lesz.
- Csökkentett párnázás, mert a hőzsebek kisebbek lesznek.
- A nyomat több anyagot igényel, és ennek eredményeként nehezebb lesz.
- A nyomtatás tovább tart.
