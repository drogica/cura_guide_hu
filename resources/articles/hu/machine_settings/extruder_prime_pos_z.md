# Extruder Prime Z pozíció

Ha a [prime blob](../platform_adhesion/prime_blob_enable.md) engedélyezve van, ez a beállítás azt a Z-koordinátát jelzi, amelynél a prime blob mozgása elindul. Cura a prime blob végrehajtása előtt ebbe a pozícióba lép.

Az X és Y koordinátákkal ellentétben ez egy gépi beállítás. Ennek az az oka, hogy az alapozás aktusának fix Z koordinátája van. Az elsődleges folt létrehozásához a fúvókának az építőlemezre kell mozdulnia, és talán egy kicsit fel-le kell mozognia. Az [X](../platform_adhesion/extruder_prime_pos_x.md) és [az Y](../platform_adhesion/extruder_prime_pos_y.md) normál beállításokkal választható a prime blob pozíciójának mozgatásához, ha az összeállító lemezen a hely korlátozó, de a Z koordináta nem.

Az egyetlen dolog, amit ez megváltoztat, az a Z koordináta, amelyre Cura parancsot ad a fúvókának, hogy lépjen a prime blob parancs végrehajtása előtt.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
