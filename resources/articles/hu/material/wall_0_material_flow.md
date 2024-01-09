# Külső faláramlás

Ez a beállítás csak a külső fal áramlási sebességét állítja be. A külső fal áramlási sebessége a belső falak áramlási sebességétől külön állítható.

Az áramlási sebesség beállítása a külső fal alatt egy ütközőrés módszer az extrudálási sebességgel vagy a méretpontossággal kapcsolatos problémák megoldására. Ugyanez a hatás érhető el a [külső falvonal szélessége](../resolution/wall_line_width_0.md) és [a külső fal beillesztése](../shell/wall_0_inset.md) beállításainak módosításával is, de ez a beállítás intuitívabb módja lehet a kezdeti hangolásnak.

Ha csak a külső falnál van probléma az extrudálási sebességgel, akkor jobb, ha megnézi a [nyomtatási sebességet](../speed/speed_wall_0.md) és [a nyomtatási hőmérsékletet](material_print_temperature.md) . Lehet, hogy az anyag nem kap elég lendületet a fúvókán, és a nagyobb nyomtatási sebesség segíthet. Lehet, hogy a vonalak túl vékonyak ahhoz, hogy megfelelően kihúzódjanak. Lehet, hogy az anyag túl hideg vagy túl forró.

Ha probléma van a méretpontossággal, jobb, ha megnézi [a vonalszélességet](../resolution/wall_line_width_0.md) , [a vízszintes kiterjedést](../shell/xy_offset.md) és a [nyomtatási sorrendet](../shell/outer_inset_first.md) .
