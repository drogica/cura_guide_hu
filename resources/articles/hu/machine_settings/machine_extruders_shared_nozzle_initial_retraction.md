# Megosztott fúvóka kezdeti visszahúzása

Ha egy nyomtató extruderei [egy fúvókán osztoznak](machine_extruders_share_nozzle.md) , a Cura nem feltételezi, hogy minden extruder a fúvóka hegyénél lévő izzószálból indul ki. Ez a beállítás azt jelzi, hogy a fúvókától milyen messze kezdődik az izzószál. Előfordulhat, hogy az izzószál a [fúvókakapcsoló visszahúzási távolságától](../dual/switch_extruder_retraction_amount.md) eltérő távolságból indul, mivel a szál távolabb tárolható, amíg a nyomtató inaktív volt, mint amikor az extruder készenlétben áll a nyomtatás alatt.

![Az inaktív izzószál távolsága a nyomtatás előtt](../images/machine_extruders_shared_nozzle_initial_retraction.svg)

A Cura ezt fogja használni annak biztosítására, hogy az izzószál a fúvóka hegyén legyen, mielőtt megkezdi az első extruderkapcsoló feltöltését.
