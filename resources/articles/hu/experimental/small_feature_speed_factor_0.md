# Kis jellemző kezdeti rétegsebesség

A [Small Feature Max Length](small_feature_max_length.md) értéknél rövidebb kontúrok csökkentett sebességgel nyomtathatók. Ezzel a beállítással megadhatja a sebességet, amellyel ezeket a kontúrokat az első rétegre kell nyomtatni, [a normál nyomtatási sebesség](../speed/speed_wall.md) tényezőjeként. Ez külön konfigurálható a [többi réteg](small_feature_speed_factor.md) kis jellemzőinek nyomtatási sebességétől.

A kis kontúroknak nincs sok felületük ahhoz, hogy az építőlemezhez tapadjanak. Különösen, ha [a falakat a kitöltés előtt nyomtatja](../infill/infill_before_walls.md) , a kis lyukak falai gyakran csak apró körök, amelyek az építőlemezen helyezkednek el. Ha a fúvóka később egy utazás során elüti őket, leszakadhatnak az építőlemezről. Emiatt ezeknek a kis kontúroknak a nyomtatási sebessége csökkenthető a többi kontúrhoz képest. Ez lehetővé teszi, hogy az anyag jobban kifolyjon, és jobban összeolvadjon az építőlemezzel, csökkentve annak esélyét, hogy lehúzzák őket az építőlemezről.

Ezen kis kontúrok nyomtatási sebességének csökkentése nagyon csekély negatív hatással van a nyomtatási sebességre. Szerencsére, mivel ezek a kontúrok definíció szerint kicsik, és csak az első rétegre vonatkozik, a teljes hozzáadott nyomtatási idő nem jelentős.
