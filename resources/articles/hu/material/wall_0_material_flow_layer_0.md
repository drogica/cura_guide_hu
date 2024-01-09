# Kezdeti réteg külső faláramlás

A kezdeti réteg áramlása módosítható az [Initial Layer Flow](material_flow_layer_0.md) beállítással, de ez a beállítás lehetővé teszi a kezdeti réteg finomabb részleteinek szabályozását azáltal, hogy az első rétegen csak a külső fal áramlását módosítja.

A kezdeti réteg egyes részei nagyobb valószínűséggel leválnak az építőlemezről, mint mások. A nyomat első sorai a legveszélyesebbek. Ezzel a beállítással módosíthatja a külső falat nagyobb áramlásra, hogy jobban rögzítse az építőlemezhez. Ez akkor hasznos, ha nincs perem a nyomatban, mert a külső fal egyetlen, laza vonalként kerül rányomtatásra az építőlemezre, viszonylag kis felülettel, amelyhez ragaszkodni lehet.

Csak a külső fal áramlási sebességének megváltoztatásával elkerülhetők a nagy áramlási sebességgel kapcsolatos problémák, például [a túlextrudálás](../troubleshooting/overextrusion.md) .
