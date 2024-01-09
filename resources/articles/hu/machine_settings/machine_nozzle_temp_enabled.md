# Engedélyezze a fúvóka hőmérséklet-szabályozását

Ha ez a beállítás le van tiltva, a Cura nem ad ki semmilyen hőmérsékleti parancsot a g-kódnak. Ehelyett a Cura a nyomtató firmware-ére bízza a fúvókák felmelegítését a nyomtatás előtt.

Működésében hasonló [a Has Heated Build Plate-](machine_heated_bed.md) hez. Ha ez a beállítás le van tiltva, a hőmérséklet-szabályozási beállítások, például [a Nyomtatási hőmérséklet](../material/material_print_temperature.md) nem jelennek meg a felhasználó számára.

Ennek ideiglenes letiltása felhasználható a nyomtatás száraz futtatására. Ehhez [ki kell kapcsolni az építőlemezt](machine_heated_bed.md) , [az építési térfogat fűtését](machine_heated_build_volume.md) , és az [áramlási sebességet](../material/material_flow.md) 0%-ra kell állítani.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
