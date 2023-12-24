# Kilógó falszög

Ez a beállítás azt a küszöbszöget jelzi, amely után a fal „kilógó falként” lesz megjelölve. Ezek a túlnyúló falak eltérő sebességgel nyomtathatók a [Túlnyúló fal sebessége](wall_overhang_speed_factor.md) beállítással.

Ha ez a beállítás 0°-ra van állítva, a rendszer minden falat kilógó falként kezel. Ha ez a beállítás 90°-ra van állítva, a rendszer egyetlen falat sem fog kilógó falként kezelni. A támasztékon nyugvó falakat sem kezeljük túlnyúló falként.

Ennek a funkciónak az a célja, hogy jobb kinyúlási tulajdonságokat biztosítson azokon a területeken, amelyeket szinte [támogatásra](../support/support_enable.md) szorulnának, de nem egészen. Ahelyett, hogy több időt és anyagot költene a támasztékokra és a felület hegesedésére a támaszték eltávolításakor, dönthet úgy, hogy ezeket a túlnyúló falakat egy kicsit lassabban nyomtatja, és valamivel magasabbra állíthatja a [támogatás túlnyúlási szögét](../support/support_angle.md) . Ezzel a nyomtatás szakaszosabb megközelítését éri el, és jobban növeli a túlnyúlási szögeket.

Ha ezt a beállítást magasabbra állítja, mint a Támaszték túlnyúlási szöge, jelentősen csökkenti ennek a funkciónak a hatását, mivel a támaszték tetején lévő falak nincsenek túlnyúló falként jelölve, így minden olyan falat, amely túlnyúló falnak tekintendő túlnyúlási szögben nyomtat, szintén támogatott, és nem nyomtat különböző sebességgel. Ennek a funkciónak azonban akkor is van hatása, ha a támogatás le van tiltva, vagy a túlnyúlás olyan részein, amelyek más okok miatt nem támogatottak, például [a minimális támogatási terület](../support/minimum_support_area.md) .
