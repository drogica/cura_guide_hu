# Alternatív fali irányok

Ha engedélyezve van, ez a beállítás a falak tekercselésének irányát az óramutató járásával megegyező és azzal ellentétes irányba váltja.

Az első belső fal a külsővel ellentétes irányba, a második belső fal pedig ismét az ellenkező irányba kerül nyomtatásra. Sőt, a következő rétegen is szemben fog indulni, így az egymásra rakott falak is váltakoznak.

A nyomtatási irány váltakozása csökkenti a modellen belüli belső feszültségek hatását, csökkentve a [vetemedés](../troubleshooting/warping.md) hatását. Bármely vonal nyomtatása során a fúvóka meglehetősen erősen meghúzza az olvadt anyag zsinórját, ami megfeszíti a műanyagot. A szilárdulás során ez a feszültség deformálhatja a modellt. Ha a szomszédos vonalat az ellenkező irányba nyomtatjuk, akkor ezt a feszültséget ellensúlyozzák a szomszédos vonalak ellenkező irányba húzása. A feszültség erejét ellentétes irányú feszültség ellensúlyozza.

A falirányok váltakozásának hátránya a nyomtató portáljában kialakuló hiszterézis. Ha holtjáték van a nyomtató tengelyein vagy tárcsáiban, akkor az átlós vonalak kissé eltérő helyen jelennek meg az ellenkező irányú nyomtatáskor. Ennek eredményeként a fal kevésbé lesz sima, és a nyomtatási méretek kevésbé pontosak. Egy jól beállított nyomtató nem mutatja ezt a hatást, így ha a nyomtató megfeszített szíjakkal, tárcsákkal és pontos alkatrészekkel rendelkezik, a falirányok váltogatása valószínűleg csak előnyökkel jár.

[Belülről kifelé történő nyomtatáskor](../shell/inset_direction.md) ez a beállítás jobban láthatóvá teszi a fal varrását, és némi csengetést okoz, mivel a fúvóka közvetlenül a külső fal kezdete előtt teljes 180°-os elfordulást okoz, ami vibrációt okoz. Ez nem szembetűnő hatás, ha kívülről befelé nyomtat.
