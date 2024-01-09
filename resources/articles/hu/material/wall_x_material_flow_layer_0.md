# Kezdeti réteg belső faláramlás

A kezdeti réteg áramlása módosítható az [Initial Layer Flow](material_flow_layer_0.md) beállítással, de ez a beállítás lehetővé teszi a kezdeti réteg finomabb részleteinek szabályozását azáltal, hogy az első rétegen csak a belső falak áramlását módosítja.

A kezdeti réteg egyes részei nagyobb valószínűséggel leválnak az építőlemezről, mint mások. A nyomat első sorai a legveszélyesebbek. Ezzel a beállítással módosíthatja a belső falakat, hogy nagyobb áramlást biztosítsanak, hogy jobban rögzítsék az építőlemezhez. Ez különösen akkor hasznos, ha a belső falakat a külső fal előtt nyomtatja, mert ekkor az első belső fal egyetlen, laza vonalként kerül nyomtatásra, mielőtt a külső falhoz és a karimához rögzítené.

Csak a belső fal áramlási sebességének megváltoztatásával elkerülhetők a nagy áramlási sebességgel kapcsolatos problémák, például [az elefántláb](../troubleshooting/elephants_foot.md) .
