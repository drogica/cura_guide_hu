# Automatikus hőmérséklet

Ha gyorsabban nyomtat, a legjobb, ha valamivel magasabb hőmérsékleten nyomtat. Ez folyékonyabbá teszi a hőre lágyuló műanyagot, ami lehetővé teszi, hogy gyorsabban kifolyjon a fúvóka nyílásán. Ez a beállítás automatikusan beállítja a hőmérsékletet a fúvókából kilépő anyag átlagos áramlási sebességétől függően.

Ha tudni szeretné, hogy a hőmérsékletet mennyire kell beállítani, az [áramlási hőmérséklet grafikonja](material_flow_temp_graph.md) hivatkozik. Az áramlási sebességet köbmilliméter per másodpercben számítják ki. Ha ezt az előremenő hőmérséklet összefüggésbe helyezzük, akkor egy bizonyos hőmérsékletet kapunk. Ez a hőmérséklet lesz nyomtatási hőmérsékletként használatos. Ha ez a beállítás aktiválva van, a szokásos [nyomtatási hőmérséklet-](../material/material_print_temperature.md) beállítás többé nem kerül alkalmazásra az áramlási sebességből számított hőmérséklet helyett.

Ennek a beállításnak a célja a jobb nyomtatási minőség elérése, csökkentve a túl- és alulextrudálást, ha a nyomaton belül nagy áramlási változások következnek be. Ennek gyakori esete a bőr és a kitöltés közötti határ. Mivel a bőrt általában sokkal lassabban nyomtatják, mint a kitöltést, azokat a rétegeket, ahol sok a kitöltés, valamivel magasabb hőmérsékleten kell nyomtatni, hogy az anyag megfelelően extrudálható legyen a kitöltés nyomtatása során.

Sok nyomtató esetében a nyomtató fúvókájában lévő hőmérsékletet szabályozó PID-szabályozó hajlamos túlreagálni, ha rövid időn belül sok hőmérséklet-változás következik be. Emiatt a nyomtatási hőmérséklet nagyon pontatlan lehet ennek a beállításnak a használatakor.

**Ez a beállítás jelenleg nem látható a Cura felületén, és nem is aktiválható.**
