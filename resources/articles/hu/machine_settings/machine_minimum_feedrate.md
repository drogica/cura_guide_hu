# Minimális előtolás

A 3D nyomtatókhoz készült Marlin firmware, amelyből a legtöbb nyomtató firmware származik, minden mozgásához rendelkezik egy minimális sebességgel. Ez a beállítás azt jelzi, hogy mi a minimális sebesség a nyomtató firmware-éhez.

A minimális sebesség egy olyan beállítás, amely megakadályozza a firmware-ben a nullával való osztás miatti hibákat. A firmware-nek ki kell számítania a lépések közötti időintervallumot, hogy a megfelelő időzítéssel jelet küldjön a motoroknak. Ha a motornak 0 sebességgel kell mozognia (azaz állni kell), ez végtelen időintervallum lenne, amit a firmware nem tud jól kezelni. Ez csak akkor érvényes, ha a nyomtató egyik motorja sem forog. Például X irányban haladva az Y tengelyt vezérlő motor továbbra sem forog, de a léptetőmotorok bonyolultsága miatt itt nem érvényes a minimális előtolás.

A Cura ezt a minimális előtolási sebességet használja a helyes időbecslések előállításához. A nyomtatás elején vagy szünet utáni gyorsításkor, illetve a nyomtatás végén vagy szünet előtti leállásig történő lassításkor alkalmazzák.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
