# Maximális gyorsulás Y

Ez a beállítás azt a maximális gyorsulást jelzi, amelyet a nyomtató motorja és kerete képes kezelni Y irányban, a nyomtató firmware-jének megfelelően.

Ez a beállítás csak a pontos időbecslések készítésére szolgál. A Cura által beállított [gyorsulásnak](../speed/acceleration_print.md) nincs határa, de a Cura feltételezi, hogy a firmware tengelyenként beállít egy bizonyos határt. Ha az Y tengely gyorsulása meghaladja ezt a beállítást, akkor ezeknek a mozgásoknak a becsült ideje úgy lesz módosítva, hogy feltételezze, hogy a firmware korlátozza a gyorsulást. A teljes gyorsulás még mindig nagyobb lehet, ha egyszerre több tengellyel átlósan gyorsítunk.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
