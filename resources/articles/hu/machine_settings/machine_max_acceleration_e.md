# Maximális izzószálgyorsulás

Ez a beállítás azt a maximális gyorsulást jelzi, amelyet a nyomtató adagolómotorjai kezelnek, a nyomtató firmware-jének megfelelően.

Ez a beállítás csak a pontos időbecslések készítésére szolgál. A Cura által beállított [gyorsulásnak](../speed/acceleration_print.md) nincs határa, de a Cura feltételezi, hogy a firmware tengelyenként beállít egy bizonyos határt. Ha az adagoló gyorsulása meghaladja ezt a beállítást, a mozgások becsült ideje úgy lesz módosítva, hogy feltételezze, hogy a firmware korlátozza a gyorsulást. A teljes gyorsulás még mindig nagyobb lehet, ha egyszerre több tengellyel átlósan gyorsítunk.

Elég gyakori, hogy a feeder gyorsulási határait eltalálják, hiszen (firmware-től függően) a Cura által beállított gyorsulás az adagolót is érinti. Ezért kulcsfontosságú, hogy ez a beállítás helyesen legyen konfigurálva, hogy a visszahúzásokhoz megfelelő időbecsléseket kapjunk.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
