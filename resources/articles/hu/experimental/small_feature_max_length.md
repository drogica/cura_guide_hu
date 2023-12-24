# Kis jellemző Max Hossz

A nyomat apró részletei gyakran nagyon fontosak a méret szempontjából. Ez a beállítás a nagyobb pontosság elérése érdekében lassabban nyomtatja ki a kis lyukakat a nyomaton.

Ha a nyomatban lévő lyuk kerülete kisebb, mint ez a beállítás jelzi, a lyuk kerületének nyomtatási sebessége megszorozódik a [kis jellemző sebesség](small_feature_speed_factor.md) faktorával (általában csökkentve). Ez a beállítás egy másik módja a [kis lyuk maximális méretének](small_hole_max_size.md) megközelítésének, amely általánosabb, mint a kör alakú lyukak esetében.

Ennek a funkciónak a gyakori felhasználási esete a csavarlyukak nagyon pontos méretű nyomtatása. Kis lyukak nyomtatása során a gyöngy hajlamos a fúvókával együtt a sarokba húzódni. Ha a sarok nagyon éles, mint például a kis lyukaknál, akkor a lyuk kisebb lesz. Lassabb nyomtatás esetén ez a húzóerő csökken, mert az anyagnak több ideje van a beépüléshez, és mert a mechanikai húzás egyszerűen alacsonyabb.

Ennek a beállításnak a növelésével több kontúr lesz megjelölve "kis jellemzőként". A nyomat lyukainak nagyobb része lassabban nyomtatódik ki. Ez a lyukak pontosabb nyomtatását eredményezi, de megnöveli a nyomtatási időt.
