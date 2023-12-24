# Felszíni mód

Normális esetben a Cura keresztmetszeteket készít a háló összes háromszögéből. Ezeket a vonalszakaszokat hurkokat fűzik össze. A nem zárt hurkok el lesznek vetve.

Ez a beállítás szabályozza, hogy mi történjen ezekkel a nem zárt hurkokkal. Ha „Normal”-ra van állítva, a rendszer elveti őket. Ha „Felület”-re van állítva, az összes keresztmetszet körvonalként kerül kinyomtatásra. Ha „Mindkettő”-re van állítva, a zárt körvonalak normál módon, de a lezáratlanok külön-külön kerülnek kinyomtatásra extra falként.

<!--screenshot {
"image_path": "magic_mesh_surface_mode_normal.png",
"models": [{"script": "extra_surface.py"}],
"camera_position": [66, 129, 124],
"settings": {
    "magic_mesh_surface_mode": "normal"
},
"colours": 32
}-->

<!--screenshot {
"image_path": "magic_mesh_surface_mode_surface.png",
"models": [{"script": "extra_surface.py"}],
"camera_position": [66, 129, 124],
"settings": {
    "magic_mesh_surface_mode": "surface"
},
"colours": 32
}-->

<!--screenshot {
"image_path": "magic_mesh_surface_mode_both.png",
"models": [{"script": "extra_surface.py"}],
"camera_position": [66, 129, 124],
"settings": {
    "magic_mesh_surface_mode": "both"
},
"colours": 32
}-->

![A normál módban a jobb oldalon nincs egyetlen záratlan felület](../images/magic_mesh_surface_mode_normal.png)![A Felületi mód csak a felületeket nyomtatja, anélkül, hogy zárt kötetként kezelné azokat](../images/magic_mesh_surface_mode_surface.png)![A kötetek és a jobb oldali extra záratlan felület nyomtatása](../images/magic_mesh_surface_mode_both.png)

A nyomtatott extra felületek csak a függőleges felületeket tartalmazzák egyetlen vonalként. Vízszintes felületekre nincs kitöltési technika, mivel a felületek nem zárt sokszögek. Nem tölthetők meg, mivel nincs bent. Nem lehet felső, alsó, kitöltés vagy támaszték. Csak egy sor.

Az extra felületek úgy lesznek kinyomtatva, mintha külső falak lennének, így hatással lesz rájuk a külső fal nyomtatási sebessége, vonalszélessége stb. Ezeket a felületeket olyan vonallal is nyomtatja, amely pontosan a felület közepére van állítva, ahelyett, hogy a vonalat a modell belseje mentén igazítja. Ez azt jelenti, hogy fél vonalszélességgel nyúlik a felület mindkét oldalán. Ez azért történik, mert nem egyértelmű, hogy a felület melyik oldala a modell belseje. A nyomat mérete nem lesz pontos. Ha, mint a fenti képernyőképen, az extra felület egy normál, szilárd felülethez van igazítva, és a „Mindkettő” opciót használja a hiányzó falak kiegészítésére, akkor a rétegek nem illeszkednek megfelelően.

**Ha a normál köteteket és az extra felületeket is nyomtatja, ne feledje, hogy a kötetek nyomtatása úgy történik, hogy a külső fal teljesen a köteten belül van. Az extra felületeken a vonal a felület közepén van nyomtatva, mindkét oldalon a vonal szélességének felével. Ha egy extra felületet egy zárt kötet felületéhez igazítunk, mint a fenti képeken, akkor a felület fél vonalszélességgel eltolódik. Hiszen az extra felületnek nincs belseje, ahová mozdulni lehetne.**
