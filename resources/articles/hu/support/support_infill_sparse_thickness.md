# Támogassa a kitöltőréteg vastagságát

Mivel a támogatás vizuális minősége és felbontása nem fontos, a nyomtatási idő csökkentése érdekében vastagabb rétegeket is használhat a támogatáshoz. Ez a beállítás konfigurálja, hogy milyen vastagságúak legyenek azok a rétegek, amelyekkel a hordozó nyomtatva lesz.

Rétegnézetben úgy fog kinézni, mintha a támasztóvonalak sokkal szélesebbek lettek volna. A tényleges nyomtatáskor a tartóvonalak tovább ereszkednek, ahelyett, hogy vízszintesen szétterülnének.

<!--screenshot {
"image_path": "support_infill_sparse_thickness.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["scale(0.5)", "rotateX(90)"]
    }
],
"camera_position": [18, 43, 19],
"settings": {
    "support_enable": true,
    "support_infill_sparse_thickness": 0.24
},
"layer": 148,
"colours": 64
}-->

![A Support Kitöltési réteg vastagsága a rétegmagasság háromszorosára van beállítva](../images/support_infill_sparse_thickness.png)

A kitöltő réteg vastagságának a szokásos rétegmagasság többszörösének kell lennie. Ha nem, akkor a rendszer a legközelebbi rétegmagasságra kerekíti.

Ez a beállítás nem vonatkozik a tartótetőre vagy a padlóra, csak a tartó fő szerkezetére.

Ez a beállítás különösen akkor hasznos, ha a hordozót a nyomat többi részétől eltérő anyaggal nyomtatja, és még inkább akkor, ha az anyag nehezen extrudálható, például PVA. Mivel a támaszték nincs minden rétegen extrudálva, a nyomtatónak nem kell olyan gyakran váltania az extrudert, így sok időt takaríthat meg. Mivel több anyagot extrudálnak a nyomtatott rétegeken, megbízhatóbban nyomtathatók azok az anyagok, amelyeknek időbe telik az áramlás beindítása.

Legyen óvatos, ha ezt túl sokat növeli. Támogatásra és visszakapcsoláskor a fúvókán keresztüli áramlási sebességnek jelentősen fel kell gyorsulnia és le kell lassulnia. Ebben van némi késés, így túl keveset fog kinyomni a támogatás elején, és túl sokat a támogatás vége után.
