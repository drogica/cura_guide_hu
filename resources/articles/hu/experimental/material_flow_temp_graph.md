# Áramlási hőmérséklet grafikon

Ha gyorsabban nyomtat, a legjobb, ha valamivel magasabb hőmérsékleten nyomtat. Ez a hőre lágyuló műanyagot folyékonyabbá teszi, lehetővé téve, hogy gyorsabban kifolyjon a fúvóka nyílásán. Ha [az Auto Temperature](material_flow_dependent_temperature.md) engedélyezve van, ez a beállítás minden áramlási sebességhez meghatározza, hogy milyen hőmérsékleten kell nyomtatni az anyagot. Ezután minden rétegre átlagolják az áramlási sebességet, hogy meghatározzák az adott réteg hőmérsékletét.

Az áramlási sebességet köbmilliméter per másodpercben számítják ki, egy teljes rétegre átlagolva. A hőmérséklet Celsius-fokban van megadva. Ennek a beállításnak a koordináták vesszővel elválasztott listájának kell lennie. Minden koordináta `[<flow>, <temperature>]` alakú.

Ennek a beállításnak a célja a jobb nyomtatási minőség elérése, csökkentve a túl- és alulextrudálást, ha a nyomaton belül nagy áramlási változások következnek be. Ennek gyakori esete a bőr és a kitöltés közötti határ. Mivel a bőrt általában sokkal lassabban nyomtatják, mint a kitöltést, azokat a rétegeket, ahol sok a kitöltés, valamivel magasabb hőmérsékleten kell nyomtatni, hogy az anyag megfelelően extrudálható legyen a kitöltés nyomtatása során.

Sok nyomtató esetében a nyomtató fúvókájában lévő hőmérsékletet szabályozó PID-szabályozó hajlamos túlreagálni, ha rövid időn belül sok hőmérséklet-változás következik be. Emiatt a nyomtatási hőmérséklet nagyon pontatlan lehet ennek a beállításnak a használatakor.

**Ez a beállítás jelenleg nem látható a Cura felületén, és nem is aktiválható.**
