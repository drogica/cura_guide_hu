# Áramlási sebesség kompenzáció Max. extrudálási eltolás

Az áramlási sebesség kompenzáció a Marlin [Linear Advance](http://marlinfw.org/docs/features/lin_advance.html) funkciójához hasonló kísérlet. Az áramlási sebesség kompenzáció célja az alul- és túlextrudálás kompenzálása, amikor az anyag áramlási sebessége megváltozik a fúvókán. Ez a beállítás korlátozza azt a távolságot, ameddig az anyagot vissza kell húzni vagy előre kell tolni az áramlásváltozások kompenzálására.

Az áramlási sebesség kompenzációja nyomtatás közben tovább mozgatja az izzószálat eredeti helyzetéből, vagy hátrébb. Ez a beállítás korlátozza, hogy az izzószál milyen messzire mozduljon el eredeti helyzetétől.

A kompenzáció extra izzószál-mozgásokat eredményez a nyomat során. Ezek időről időre lelassítják a nyomtatófejet az izzószál mozgatásához. Ennek hatásának csökkentése érdekében korlátozhatja az izzószál mozgási távolságát. Ez megakadályozza, hogy a nyomtatófejnek le kell lassítania, hogy az adagoló lépést tudjon tartani. Ez azonban csökkenti az áramlási sebesség kompenzáció hatékonyságát.
