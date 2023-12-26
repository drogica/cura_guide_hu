# Kitöltési minta

A kitöltési minta egy olyan struktúrát határoz meg, amely az objektum térfogatának kitöltésére szolgál. Különféle minták állnak rendelkezésre, amelyek mindegyikének megvannak a maga előnyei. Néhányuk nagyon speciális alkalmazásokra specializálódott.

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

## Rács

![Rács](../images/infill_pattern_grid.png)

A rácskitöltési minta két merőleges vonalkészletet hoz létre. Ez együtt négyzetmintát alkot.

- Legerősebb minta függőleges irányban.
- Meglehetősen erős a vonalak két irányában.
- Nem olyan erős az átlóban.
- Nagyon jól megtámasztja a felső felületet. Felülete nagyon sima lesz.

<!--screenshot {
"image_path": "infill_pattern_lines.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "lines"
},
"colours": 64
}-->

## Vonalak

![Vonalak](../images/infill_pattern_lines.png)

A vonalminta párhuzamos vonalakat hoz létre. Alapértelmezés szerint a vonalminta merőlegesen váltogatja irányát rétegről rétegre, ami első pillantásra úgy néz ki, mint a rácsminta. Ez azonban módosítható a [Kitöltési vonal irányai](infill_angles.md) beállítással.

<!--if cura_version<4.12:* The best pattern for a smooth top surface together with zigzag, since the distance between the lines is smallest.-->

- Függőleges irányban gyengék, mivel a rétegeknek csak kis pontjai vannak, amelyekben egymáshoz tapadnak.
- Vízszintes irányban rendkívül gyenge lesz, kivéve azt az egy irányt, amelyben a vonalak vannak. De még ebben az irányban sem ellenáll a nyírásnak, így terhelés alatt meglehetősen gyorsan meghibásodik.

<!--screenshot {
"image_path": "infill_pattern_triangles.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "triangles"
},
"colours": 64
}-->

## Háromszögek

![Háromszögek](../images/infill_pattern_triangles.png)

A háromszög minta három vonalkészletet hoz létre három különböző irányban. Ez együtt háromszögmintát alkot.

- Nagyon ellenáll a nyírásnak.
- Körülbelül azonos erősségű minden vízszintes irányban.
- A felső vonalaknak meglehetősen hosszan kell áthidalniuk, így sok felső bőrrétegre van szükség ahhoz, hogy egyenletes felső felületet kapjanak.
- Az áramlás jelentősen megszakad a kereszteződésekben, ami viszonylag alacsony szilárdságot eredményez magas feltöltési arány mellett.

<!--screenshot {
"image_path": "infill_pattern_trihexagon.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "trihexagon"
},
"colours": 64
}-->

## Három hatszög

![Három hatszög](../images/infill_pattern_trihexagon.png)

A három hatszögletű minta három vonalkészletet hoz létre három különböző irányban, csakúgy, mint a háromszögek mintája, de eltolják egymástól, hogy ne metsszék egymást ugyanabban a helyzetben.

- Legerősebb minta vízszintes irányban.
- Körülbelül azonos erősségű minden vízszintes irányban.
- Nagyon ellenáll a nyírásnak.
- A felső vonalaknak nagyon hosszan kell áthidalniuk, ezért sok felső bőrrétegre van szükség ahhoz, hogy egyenletes felső felületet kapjanak.

<!--screenshot {
"image_path": "infill_pattern_cubic.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "cubic",
    "infill_sparse_density": 19
},
"colours": 64
}-->

## Kocka alakú

![Kocka alakú](../images/infill_pattern_cubic.png)

A kockaminta kockákat hoz létre, egy 3 dimenziós mintát. A kockák egy sarokban állnak, így a belső felületek kilógása nélkül nyomtathatók.

- Körülbelül azonos erősségű minden irányban, beleértve a függőleges irányt is.
- Meglehetősen erős minden irányban.
- Csökkenti a párnázás hatását, mivel nem hoz létre hosszú függőleges forró levegőzsebeket.

<!--screenshot {
"image_path": "infill_pattern_cubic_subdivision.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "cubicsubdiv",
    "infill_sparse_density": 50
},
"layer": 240,
"colours": 64
}-->

## Köbös alosztály

![Köbös felosztás](../images/infill_pattern_cubic_subdivision.png)

A kockafelosztási minta kockákat hoz létre, egy 3-dimenziós mintát. A kockák egy sarokban állnak, így a belső felületek kilógása nélkül nyomtathatók. Ez a minta azonban nagyobb kockákat eredményez a kötet belseje felé, ami anyagot takarít meg. Azokon a helyeken hagyja el a kitöltő sorokat, ahol a legkevésbé hasznosak.

Ez a minta a kívántnál alacsonyabb kitöltési sűrűséget eredményezhet. Ennek a mintának a használatakor célszerű drasztikusan növelni a kitöltési sűrűséget. Az optimalizálás a legjobban magas kitöltési arány mellett működik.

Algoritmikusan ezt a mintát úgy állítják elő, hogy egy óriási kockát hoznak létre a teljes kötet körül, majd ezt a kockát 8 alkockára osztják fel, amikor falnak ütközik. Ez ezután megismétlődik, így a falba ütköző alkockák újra és újra felosztásra kerülnek. Ez addig ismétlődik, amíg el nem éri a betöltési vonal távolságát.

- A legerősebb minta súly és nyomtatási idő szerint.
- Körülbelül azonos erősségű minden irányban, beleértve a függőleges irányt is.
- A tölteléket vékony darabokra sűríti.
- Csökkenti a párnázás hatását, mivel nem hoz létre hosszú függőleges forró levegőzsebeket.
- Ha megnövelt kitöltéssűrűséget használ, akkor a kitöltés nem nagyon süt át a falakon, így jobb felületi minőség érhető el egyenlő nyomtatási idő mellett.
- Bevezeti a visszahúzásokat, ami nem működik jól rugalmas vagy folyós anyagok esetén.
- Tovább tart a szeletelés.

<!--screenshot {
"image_path": "infill_pattern_octet.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "tetrahedral",
    "infill_sparse_density": 21
},
"colours": 64
}-->

## Oktett

![Oktett](../images/infill_pattern_octet.png)

Az oktett minta szabályos tetraéderek és kockák kombinációját hozza létre, egy 3 dimenziós mintát. Időnként több kitöltési sor kerül egymás mellé.

- Erős belső keretet hoz létre, ahol több párhuzamos vonal érintkezik. A terhelés gyorsan eloszlik a belső keret felé.
- Erős közepes vastagságú, körülbelül egy centiméteres modelleken.
- Csökkenti a párnázás hatását, mivel nem hoz létre hosszú függőleges forró levegőzsebeket.
- Nagyon hosszú áthidaló távolságot eredményez a felső bőrön, ami csökkenti a felső felület minőségét.

<!--screenshot {
"image_path": "infill_pattern_quarter_cubic.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "quarter_cubic",
    "infill_sparse_density": 21
},
"colours": 64
}-->

## Negyed köbös

![Negyed köbös](../images/infill_pattern_quarter_cubic.png)

A negyed köbös mintázat háromdimenziós tesszelációt hoz létre, amely tetraéderekből és csonka tetraéderekből áll. Időnként több kitöltő sor kerül egymás mellé.

- Két különálló belső keretet hoz létre, hasonlóan az oktetthez, ahol több párhuzamos vonal érintkezik. A terhelés gyorsan eloszlik a belső keret felé. A keretek két különböző irányba vannak elhelyezve, így külön-külön gyengébbek, de csökkentik a terhelés elosztásának távolságát ezeken a kereteken.
- Erős az alacsony, néhány milliméteres vastagságú modelleken.
- Csökkenti a párnázás hatását, mivel nem hoz létre hosszú függőleges forró levegőzsebeket.
- Nagyon hosszú áthidaló távolságot eredményez a felső bőrön, ami csökkenti a felső felület minőségét.

<!--screenshot {
"image_path": "infill_pattern_concentric.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "concentric"
},
"colours": 64
}-->

## Körkörös

![Körkörös](../images/infill_pattern_concentric.png)

A koncentrikus minta a falakkal párhuzamos gyűrűket hoz létre.

- A legerősebb kitöltési mintázat 100%-os kitöltés esetén, mivel nem csak, hogy nem metszik egymást a vonalak, hanem a vonalak úgy is vannak orientálva, hogy a vonalak nem izotróp szilárdsága elosztja a terhelést.
- A legrugalmasabb nyomatokat készíti, nagyon gyenge és egyenletes szilárdsággal minden vízszintes irányban.
- Erősebb függőleges irányban, mint vízszintes irányban.
- 100%-os kitöltési sűrűség esetén az anyag összetapadhat a közepén, csökkentve a kerek formák nyomtatásának megbízhatóságát, ahol a koncentrikus körök egy pontban találkoznak.
- Egyes formáknál a kitöltő vonalak némelyike ​​a levegőben lóghat, ami nem növeli az anyagköltséget és a nyomtatási időt.
- Ha nem 100%-os kitöltést használ, ez a leggyengébb kitöltési minta vízszintes irányban. Egyáltalán nem ad hozzá erőt.

<!--screenshot {
"image_path": "infill_pattern_zigzag.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "zigzag"
},
"colours": 64
}-->

## Cikcakk

![Cikcakk](../images/infill_pattern_zigzag.png)

A cikk-cakk kitöltési minta miatt a fúvóka cikk-cakk módon húzza a vonalakat. Ez olyan, mint a vonalak, de a vezetékek egy hosszú vonalban vannak összekötve, ami megakadályozza az áramlás megszakítását.

- A második legerősebb kitöltési minta 100%-os kitöltés esetén. Megbízhatóbban nyomtat, mint a kerek formájú koncentrikus kitöltés.
- A legjobb minta a sima felső felülethez cikkcakkal együtt, mivel a vonalak közötti távolság a legkisebb.
- Függőleges irányban meglehetősen gyenge, mivel a rétegeknek csak kis pontjaik vannak, amelyekben egymáshoz tapadnak.
- Vízszintes irányban rendkívül gyenge lesz, kivéve azt az egy irányt, amelyben a vonalak vannak. De még ebben az irányban sem ellenáll a nyírásnak, így terhelés alatt meglehetősen gyorsan meghibásodik.

<!--screenshot {
"image_path": "infill_pattern_cross.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "cross"
},
"colours": 64
}-->

## Kereszt

![Kereszt](../images/infill_pattern_cross.png)

A keresztbetöltési minta egy térkitöltő görbét hoz létre, amely olyasmit hoz létre, amely keresztnek néz ki a kötet belsejében.

- Minden vízszintes irányban egyenletesen sima, így puha és rugalmas tárgyak nyomtatásához hasznos.
- Nem hoz létre hosszú egyenes vonalakat vízszintes irányban, így ez egyenletesen sima lesz a teljes kerület mentén. Nincsenek erős pontok.
- Egyáltalán nem okoz visszahúzódást, így könnyebben nyomtathat rugalmas anyagokkal.
- Erősebb lesz függőleges irányban, mint vízszintes irányban.
- Sok időt vesz igénybe a szeletelés.
- Nagyon gyenge lesz minden vízszintes irányban.

<!--screenshot {
"image_path": "infill_pattern_cross_3d.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "cross_3d"
},
"colours": 64
}-->

## Kereszt 3D

![Kereszt 3D](../images/infill_pattern_cross_3d.png)

A keresztirányú 3D-kitöltési minta egy térkitöltő görbét hoz létre, amely olyasmit hoz létre, amely keresztnek néz ki a kötet belsejében. Ez a minta a Z tengely mentén pulzál, hogy függőleges irányban gyengébb legyen.

- Körülbelül egyenletesen sima minden irányban, vízszintesen és függőlegesen is, így ez a leghasznosabb minta puha és rugalmas tárgyak nyomtatásához.
- Nem hoz létre hosszú egyenes vonalakat, így egyenletesen simává válik az egész felületen.
- Egyáltalán nem okoz visszahúzódást, így könnyebben nyomtatható rugalmas anyagokkal.
- Sok időt vesz igénybe a szeletelés.
- Nagyon gyenge lesz minden irányban.

<!--screenshot {
"image_path": "infill_pattern_gyroid.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "gyroid"
},
"colours": 64
}-->

## Gyroid

![Gyroid](../images/infill_pattern_gyroid.png)

A giroid kitöltési minta hullámos mintát hoz létre, amely váltakozó irányokat.

- Egy térfogatot hoz létre, amely teljesen áteresztő a folyadékok számára, így ez hasznos minta az oldódó anyagok számára.
- Minden irányban egyformán erős, de nem túl merev. Ez hasznossá teszi a rugalmas anyagokhoz, de az eredmény valamivel keményebb, kevésbé csillogó lesz, mint a Cross (3D) kitöltési minták.
- Ebben a mintában nincsenek átfedő vonalak, ami megkönnyíti a nagyobb felületi feszültségű anyagokkal való nyomtatást, és nagyon megbízhatóvá és konzisztenssé teszi a kitöltést.
- Nyírásnak ellenálló.
- Sok időt vesz igénybe a szeletelése, és nagyméretű g-kód fájlokat hoz létre. Egyes nyomtatók számára nehéz lehet lépést tartani a másodpercenkénti sok g-kód utasítással, és nehéz lehet lépést tartani a túlzott soros kapcsolattal alacsony adatátviteli sebesség mellett.

<!--screenshot {
"image_path": "infill_pattern_lightning.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "lightning"
},
"colours": 64
}-->

<!--screenshot {
"image_path": "infill_pattern_lightning_side.png",
"models": [{"script": "three_cylinders.scad"}],
"camera_position": [148, 23, 126],
"settings": {
    "top_layers": 0,
    "wall_line_count": 0,
    "infill_pattern": "lightning",
    "infill_sparse_density": 30
},
"colours": 32
}-->

<!--if cura_version>=4.12-->

## Villám

![Villám](../images/infill_pattern_lightning.png)![A villámminta oldalról épül fel](../images/infill_pattern_lightning_side.png)

A villámkitöltő minta egy szaggatott minimális minta, amely csak a felső felület megtámasztását célozza. A megadott feltöltési sűrűség csak közvetlenül a feltöltési térfogat felső része alatt érhető el.

- Rengeteg időt és anyagot takarít meg azzal, hogy csak a felület alatt képződik kitöltés.
- A kitöltés sűrűségének növelése minden minta legjobb felületi minőségéhez vezet, miközben nem igényel több időt és anyagot.
- Megakadályozza, hogy a kitöltés sok helyen átsüljön a falakon, egyszerűen nincs kitöltve.
- Semmilyen mértékben nem növeli az alkatrész szilárdságát.

<!--endif-->
