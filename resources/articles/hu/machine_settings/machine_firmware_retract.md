# Firmware visszahúzás

Normális esetben a Cura visszahúzódást okoz az adagoló mozgásának szabályozásával, és megparancsolja neki, hogy mozgassa egy kicsit hátra az izzószálat. Ha ez a beállítás engedélyezve van, akkor ehelyett egy `G10` parancsot ír, ami azt jelenti, hogy a nyomtatónak vissza kell húznia az izzószálat, vagy egy `G11` parancsot a visszahúzáshoz.

A firmware-behúzások használatának választásával a nyomtató firmware-je szabályozza, hogy milyen messzire és milyen gyorsan kell visszahúzni az izzószálat. A nyomtató többet tudhat saját geometriájáról, mint a Cura, így jobban el tudja dönteni, hogyan kell visszahúzni az izzószálat. Ez azonban azt jelenti, hogy Cura már nem irányítja ezeket a visszahúzásokat, és Cura többet tud magáról a nyomatról. Lényegében a szeletelő és a firmware eltérő információkkal rendelkezik, és ez a beállítás dönti el, hogy a kettő közül melyiket kell választani.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
