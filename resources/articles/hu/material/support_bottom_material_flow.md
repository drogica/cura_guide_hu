# Támogassa a padlóáramlást

Ez a beállítás csak a támasztópadló áramlási sebességét állítja be. A támasztópadló áramlási sebessége a támaszték többi részének áramlási sebességétől külön állítható.

Az áramlási sebesség beállítása a támasztófenék alatt egy ütközőrés módszer az extrudálási sebességgel vagy a modell és a támaszték közötti tapadás problémáinak megoldására. Ugyanez a hatás érhető el a támasztópadló [vonalszélességének](../resolution/support_bottom_line_width.md) vagy [sortávolságának](../support/support_bottom_line_distance.md) beállításával, de az áramlási sebesség beállítása intuitívabb lehet.

Ha probléma van az extrudálási sebességgel, jobb, ha megnézi a [nyomtatási sebességet](../speed/speed_support_bottom.md) , [a hőmérsékletet](material_print_temperature.md) és [a vonalszélességet](../resolution/support_bottom_line_width.md) . Talán túl nagy a különbség a tartópadló és a réteg többi szerkezete között. Lehet, hogy a vonal szélessége túl vékony a megfelelő extrudáláshoz. Ha a felületet [más anyaggal](../support/support_interface_extruder_nr.md) nyomtatják , gyakori probléma az, hogy az anyag, amelyre a felület nyomtatott, nem jut elegendő időhöz, hogy megfelelően elkezdjen folyni. Ez rögzíthető egy [primer torony](../dual/prime_tower_enable.md) használatával vagy [a tartópadló területének](../support/support_bottom_offset.md) növelésével.

Ha a támasz túl jól tapad a modellhez, a [vonalszélesség](../resolution/support_bottom_line_width.md) beállítása általában hatékonyabb, mivel ez azt is eredményezi, hogy a vonalak közelebb kerülnek egymáshoz, hogy ugyanazt a támasztékkitöltési sűrűséget érjük el.
