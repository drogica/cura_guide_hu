# Kitöltőréteg vastagsága

Mivel a kitöltés rétegmagassága nem fontos a vizuális minőség szempontjából, a nyomtatási idő csökkentése érdekében vastagabb rétegeket is használhat a kitöltéshez. Ez a beállítás a kitöltési rétegek kombinálását eredményezi, mindaddig, amíg több kitöltési réteg van közvetlenül egymás felett. Ekkor egyes rétegekre nem nyomtat kitöltést, de a kombinált rétegek közül a legmagasabbra több anyagot extrudál, hogy pótolja.

Rétegnézetben úgy fog kinézni, mintha a kitöltési vonalak sokkal szélesebbek lettek volna. A tényleges nyomtatáskor a kitöltő vonalak tovább ereszkednek, ahelyett, hogy vízszintesen szétterülnének.

<!--screenshot {
"image_path": "infill_sparse_thickness.png",
"models": [{"script": "cooking_utensil_hook.scad"}],
"camera_position": [6, 51, 27],
"camera_lookat": [0, 0, 7],
"settings": {
    "layer_height": 0.2,
    "wall_line_count": 0,
    "infill_pattern": "zigzag",
    "infill_sparse_thickness": 0.6
},
"layer": 19,
"colours": 64
}-->

![A Kitöltőréteg vastagsága a rétegmagasság háromszorosára van beállítva](../images/infill_sparse_thickness.png)

A kitöltőréteg vastagságának a szokásos rétegmagasság többszörösének kell lennie. Ha nem, akkor a rendszer a legközelebbi rétegmagasságra kerekíti.

- Legyen óvatos, ha ezt túl sokat növeli. Feltöltésre és visszakapcsoláskor a fúvókán keresztüli áramlási sebességnek jelentősen fel kell gyorsulnia és le kell lassulnia. Van némi késés, ezért túl keveset extrudál a kitöltés elején és túl sokat a kitöltés végén.
- A köztes rétegekben továbbra is kisebb rétegvastagsággal nyomtat kitöltést, ahol nincs kitöltés a körülötte lévő rétegekben. Emiatt kis kitöltési vonalak jelenhetnek meg a ferde falak mellett.
