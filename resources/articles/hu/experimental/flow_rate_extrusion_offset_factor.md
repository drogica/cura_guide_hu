# Áramlási sebesség kompenzációs tényező

Az áramlási sebesség kompenzáció a Marlin [Linear Advance](http://marlinfw.org/docs/features/lin_advance.html) funkciójához hasonló kísérlet. Az áramlási sebesség kompenzáció célja az alul- és túlextrudálás kompenzálása, amikor az anyag áramlási sebessége megváltozik a fúvókán. Ez a beállítás konfigurálja a hatás nagyságát.

Az áramlási sebesség kompenzáció minden mozdulat során a következő másodpercben szükséges extra anyaggal mozgatja előre az izzószálat. Minden lépés között három lehetséges forgatókönyv lehetséges.

- Ha a két szomszédos mozgásparancs azonos áramlási sebességgel rendelkezik (mivel azonos a vonalszélességük, a rétegmagasságuk és a sebességük), akkor az előrelépés is azonos lesz. Az izzószál semmilyen irányba nem mozdul el e vonalak között.
- Ha az áramlási sebesség a következő sorral növekszik, akkor a második sor során az izzószál tovább kerül előre. Ez megnöveli a nyomást a fúvókakamrában, így az anyag gyorsabban tud extrudálni a vonal és az azt követő vonalak nyomtatása során.
- Ha az áramlási sebesség a következő sornál csökken, az izzószál visszamozdul a második sor során. Ez csökkenti a nyomást a fúvókakamrában, így az anyag lelassul a második sor és az azt követő sorok nyomtatása során.

Az a távolság, ameddig az izzószál elmozdul, megegyezik azzal az anyagmennyiséggel, amelyet a sor során másodpercenként extrudálnának (ha a vonal elég hosszú lenne egy teljes másodperc nyomtatásához). Ezzel a beállítással azonban ez a távolság beállítható. A tényező növelése erősebbé teszi a kompenzációs hatást. Ennek csökkentése gyengíti a kompenzációs hatást. A magasabb tényezők nyomtatása több időt vesz igénybe, mivel az izzószálat jobban kell mozgatni felfelé és lefelé.

Ha ez az áramlási sebesség-kompenzáció aktiválva van, a fúvókakamrában lévő nyomást jobban fel kell szerelni a közelgő áramlási sebesség kezelésére. Ez csökkentheti az alul- és túlextrudálást, és pontosabb méretet ad az objektumnak.

A kompenzációt azonban egyetlen sor alatt alkalmazzák. Ez néha egy rövid vonal lehet, amely alatt az izzószálnak nagyon gyorsan kell mozognia. Előfordulhat, hogy a nyomtatófejnek le kell lassítania, hogy az adagoló lépést tudjon tartani, ami folt megjelenését okozhatja. Néha ez hosszú sor lehet, ami csökkenti a hatás erősségét. Ez megbízhatatlanná teszi az extrudálási sebesség kompenzációjának teljes funkcióját, és ez az oka annak, hogy ez a beállítás még mindig kísérleti jellegű.
