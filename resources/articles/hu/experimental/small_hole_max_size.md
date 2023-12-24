# Kis lyuk maximális mérete

A nyomat apró részletei gyakran nagyon fontosak a méret szempontjából. Ez a beállítás a nagyobb pontosság elérése érdekében lassabban nyomtatja ki a kis lyukakat a nyomaton.

Ha egy kör alakú furat átmérője kisebb, mint ennek a beállításnak az értéke, akkor a lyuk kerületének nyomtatási sebességét a rendszer megszorozza a [kis jellemző sebesség](small_feature_speed_factor.md) faktorával (általában csökkentve). A nem kör alakú lyukak esetében a nyomtatás eltérő sebességgel történik, ha a kerület kisebb, mint az itt megadott átmérőjű kör. Lásd még [Kis jellemző Max Length](small_feature_max_length.md) ; ez az a beállítás, amelyet a szeleteléshez ténylegesen használni fognak.

Ennek a funkciónak a gyakori felhasználási esete a csavarlyukak nagyon pontos méretű nyomtatása. Kis lyukak nyomtatása során a gyöngy hajlamos a fúvókával együtt a sarokba húzódni. Ha a sarok nagyon éles, mint például a kis lyukaknál, akkor a lyuk kisebb lesz. Lassabb nyomtatás esetén ez a húzóerő csökken, mert az anyagnak több ideje van a beépüléshez, és mert a mechanikai húzás egyszerűen alacsonyabb.

Ennek a beállításnak a növelésével több kontúr lesz megjelölve "kis jellemzőként". A nyomat lyukainak nagyobb része lassabban nyomtatódik ki. Ez a lyukak pontosabb nyomtatását eredményezi, de megnöveli a nyomtatási időt.
