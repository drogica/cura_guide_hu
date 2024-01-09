# Várja meg a Build Plate Heatup-ot

Ha ez a beállítás engedélyezve van, a nyomtató minden alkalommal vár, amíg az építőlemez hőmérsékletét el nem éri.

Az építőlemez hőmérséklete általában csak az első réteg után változik, ha az [építőlemez hőmérséklete a kezdeti réteg](../material/material_bed_temperature_layer_0.md) eltér a normál [építőlemez hőmérséklettől](../material/material_bed_temperature.md) . [Egyenkénti módban történő](../blackmagic/print_sequence.md) nyomtatás esetén az építőlemez is megváltozik, amikor a következő modellnél újra a kezdeti réteggel kezdődik. Ilyen esetekben a nyomtató megvárja az új hőmérséklet elérését, mielőtt folytatná a nyomtatást.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
