# Törölje le a Z Hop-ot

Ezzel a beállítással a törlési folyamat Z ugrás közben történik. Ez a szokásos [Z ugrásoktól](../travel/retraction_hop_enabled.md) függetlenül konfigurálható.

A törlési eljárás két nagyon hosszú mozgást tartalmaz, amelyek egészen a build kötet oldaláig mennek. Az ilyen mozgások során a nyomtatófej meglehetősen nagy sebességet vehet fel, mert sok ideje van a gyorsításra. Nagy sebességnél nagyobb az esélye annak, hogy a nyomtatófej véletlenül átüti a korábban nyomtatott részeket. Ezért érdemes lehet engedélyezni a Z ugrást, még akkor is, ha a szokásos nyomtatási folyamatban ezt nem tenné meg.

A Z ugrás ebben az eljárásban attól függetlenül végrehajtásra kerül, hogy [a Z ugrások csak a korábban nyomtatott részeken vannak-e végrehajtva](../travel/retraction_hop_only_when_collides.md) , vagy vannak közöttük nyomtatott részek.
