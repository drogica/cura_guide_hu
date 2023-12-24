# Fuzzy Skin Point Distance

Ez a beállítás konfigurálja az eredeti fal mentén a mozgások közötti távolságot a homályos bőrhöz. Ha a távolság kicsi, a nyomtatófej nagyon gyakran különböző irányokba mozog a fal mentén. Magas frekvencián fog rezegni.

Kisebb távolságok esetén az érdesség finomabb lesz, ami durvább textúrát eredményez. Ez a nyomtatási időt is jelentősen befolyásolja. Simább, de göröngyös textúra létrehozásához növelheti a távolságot.

Ha a Fuzzy Skin engedélyezve van, a külső fal teljes egészében a vibrációs mozgások közötti egyenes szegmensekből áll az eredeti felület helyett. Nagy távolságok esetén előfordulhat, hogy az ívelt felületek már nem nagyon görbültek, mert a fuzzy skin hatás miatt az eredeti felbontás nagyobb volt, mint a koordináták sűrűsége.

Az algoritmikus korlátok miatt a pontok közötti távolság nem lehet túl kicsi, ha nagyon nagy a [vastagság](magic_fuzzy_skin_thickness.md) .
