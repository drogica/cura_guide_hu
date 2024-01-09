# Készenléti hőmérséklet

A Cura feltételezi, hogy a több extruderes nyomtatóknak külön fúvókái vannak, amelyek eltérő hőmérsékletűek. Amíg az egyik extruder a nyomtatással van elfoglalva, a többi fúvókát alacsonyabb hőmérsékleten kell tartani, hogy megakadályozzuk a fúvókakamrában lévő anyag lebomlását és a szivárgást. Ez az alacsonyabb hőmérséklet a készenléti hőmérséklet.

![Amíg a kék extruder nyomtat, a piros extruder lehűl a készenléti hőmérsékletre](../images/temperature_regulation.svg)

A jó készenléti hőmérséklet elég alacsony ahhoz, hogy megvédje az izzószálat a leromlástól, ami eltömítheti a fúvókát. Elég alacsony ahhoz, hogy az anyag ne szivárogjon ki a fúvókából. De elég magas ahhoz is, hogy gyorsan folytassa a nyomtatást, amikor a többi extruder elkészült.
