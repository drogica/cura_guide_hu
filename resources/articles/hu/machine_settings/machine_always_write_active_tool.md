# Mindig írjon aktív eszközt

Ez a beállítás azt jelzi, hogy bizonyos eszközparaméterekkel rendelkező g-kód parancsokat hogyan értelmezi a nyomtató. Egyes g-code parancsok tartalmazhatnak egy paramétert, amely jelzi, hogy melyik extruderre vonatkozik. Egyes firmware ezt a paramétert parancsként értelmezi, amely arra az eszközre vált, majd végrehajtja a g-kódot, míg néhány firmware ezt a paramétert parancsként értelmezi, hogy a g-kódot egy másik extruderre alkalmazza, mint az aktuálisan aktív.

Az egyetlen olyan parancs, amelyre ez vonatkozik, és amelyek a 3D nyomtatásra vonatkoznak, az `M104` és `M109` fúvókamelegítési parancsok. Vegyük a következő példát egy fűtési parancsra, amelyet az első extruder ( `T0` ) nyomtatása közben hajtanak végre:

`M104 S210 T1`

Ennek a parancsnak két lehetséges értelmezése van:

- Miközben folytatja a nyomtatást az első extruderre, kezdje el felmelegíteni a második extrudert 210 °C-ra. Ez a Marlin, a Reprap, a Sailfish és a származtatott firmware-csomagok értelmezése.
- Először váltson a második extruderre, majd melegítse fel a második extrudert 210 °C-ra. Ez a Smoothieware és a származtatott firmware értelmezése.

A Cura hőmérsékletszabályozási stratégiája miatt soha nem kell a második értelmezést végrehajtania. Ha a nyomtató a második módon értelmezi a g-code parancsot, a Cura a következő g-kódot írja helyette:

`M104 S210 T1`

`T0`

Lényegében tudja, hogy a nyomtató a parancs hatására a második extruderre kapcsol, ezért vissza kell kapcsolnia az első extruderre, hogy ott folytassa a nyomtatást.

**Mivel ez egy gépbeállítás, általában nem jelenik meg a normál beállítások listájában.**
