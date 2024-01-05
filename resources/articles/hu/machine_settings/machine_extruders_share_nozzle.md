# Extruderek Share Nozzle

Ezzel a beállítással jelezheti, hogy a nyomtatónak csak egyetlen fúvókája van, és az összes izzószál ugyanazon a fúvókán keresztül van nyomva. A Cura ezután megváltoztatja az alapozási stratégiáját.

Általában a Cura azt feltételezi, hogy a [start g-kód](machine_start_gcode.md) futtatása után minden extrudernek a fúvóka végén van az izzószála, és készen áll a nyomtatásra. Ha az extruderek egy fúvókán osztoznak, ez nem lehetséges, mivel egyszerre csak egy izzószál lehet a fúvókában. A normál feltöltési eljárás helyett egy [feltöltött folttal](../platform_adhesion/prime_blob_enable.md) vagy extra szoknyavonalakkal, a fúvókát úgy kell alapozni, mintha egy teljes extruder kapcsolóhoz lenne szükség. Ez magában foglalja a nyomtatást az [elsődleges toronyban](../dual/prime_tower_enable.md) , ha engedélyezve van.

Ha az összes extrudernek egyetlen fúvókája van, akkor magától értetődő, hogy [közös a fűtőberendezésük](machine_extruders_share_heater.md) is. A Cura azonban önmagában nem hoz létre kapcsolatot a kettő között, ezért győződjön meg róla, hogy mindkettőt engedélyezi, ha valóban a nyomtató egyetlen fúvókával és egyetlen fűtővel rendelkezik az összes extruderhez.

**Mivel ez egy gépbeállítás, általában nem jelenik meg a normál beállítások listájában. Ehhez a beállításhoz van egy jelölőnégyzet a nyomtatóbeállítások párbeszédpanelen, amely a hozzáadott nyomtatók listájában található a beállítások párbeszédablakban.**
