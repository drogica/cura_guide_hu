# Törölje Szünet

Ezzel a beállítással a fúvóka rövid ideig szünetelhet a törlési folyamat befejezése után.

A törlési eljárás meglehetősen hosszú, utazási mozdulatokhoz képest. A fúvóka egészen az építési kötet oldaláig mozdul el, és oda-vissza mozog, majd vissza kell utaznia a nyomathoz. Ez idő alatt sok lesz a szivárgás, és [hosszabb visszahúzásra](wipe_retraction_amount.md) lehet szükség. A visszahúzás után eljön egy időszak, amikor a fúvókából való kiáramlást továbbra is meg kell kezdeni. Ez a szünet lehetővé teszi, hogy a fúvóka kamrájában visszatérjen a nyomás, amikor az anyagot ismét visszahúzzák, lehetővé téve az első sor megfelelő nyomtatását jelentős alulextrudálás nélkül.

A túl hosszú szüneteltetés a fúvóka leszállási helyén folt jelenik meg. A [nyomtatási sorrendtől](../infill/infill_before_walls.md) függően ez nem feltétlenül jelentős, mivel a folt a nyomat belsejében jelenhet meg, ahol nem látható. Az ehhez a folthoz használt anyag azonban nem kerül felhasználásra a következő nyomtatott sorokhoz, ami még mindig alulextrudálást okoz. Ez a beállítás alapos hangolást igényel.
