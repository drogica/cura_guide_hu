# Minimális idő készenléti hőmérséklet

Ez a beállítás konfigurálja a készenléti állapot minimális időtartamát, ameddig a fúvóka készenléti hőmérsékletre kell hűteni. Ha a fúvókát ennél rövidebb ideig készenléti állapotra állítja be, akkor nem hűl le, hanem a [végső nyomtatási hőmérsékleten](../material/material_final_print_temperature.md) marad.

A fúvóka PID-szabályozóval rendelkezik, amely szabályozza, hogy mennyi energiát használnak fel a fúvóka felmelegítésére, hogy elérje a megfelelő hőmérsékletet. Amikor a fúvóka gyors egymásutánban nagy hőmérséklet-különbségekkel hűtést és felmelegedést kap, a PID-szabályozó hajlamos rosszul megjósolni a szükséges hőmennyiséget. Ez nagy ingadozásokat okoz a fúvóka tényleges hőmérsékletében. Ezzel megakadályozhatja, hogy [készenléti hőmérsékletre](../material/material_standby_temperature.md) menjen, ha a fúvóka nagyon rövid ideig inaktív.

Ennek a beállításnak az optimális értéke a PID szabályozó hangolásától függ. Egyes szabályozók jobban kezelik a gyors célhőmérséklet-változásokat, mint mások, ezek pedig jobban képesek kezelni a rövid készenléti időszakot. Ennek a beállításnak a csökkentése segít megelőzni az anyag lebomlását a fúvókán belül.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
