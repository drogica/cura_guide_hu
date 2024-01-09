# Támogassa a tetőáramlást

Ez a beállítás csak a tartótető áramlási sebességét állítja be. A tartótető áramlási sebessége külön állítható a tartó többi részének áramlási sebességétől.

Az áramlási sebesség beállítása a tartótető alatt egy ütközőrés módszer az extrudálási sebességgel vagy a modell és a támaszték közötti tapadás problémáinak megoldására. Ugyanez a hatás érhető el a tartótető [vonalszélességének](../resolution/support_roof_line_width.md) vagy [vonaltávolságának](../support/support_roof_line_distance.md) beállításával, de az áramlási sebesség beállítása intuitívabb lehet.

Ha probléma van az extrudálási sebességgel, jobb, ha megnézi a [nyomtatási sebességet](../speed/speed_support_roof.md) , [a hőmérsékletet](material_print_temperature.md) és [a vonalszélességet](../resolution/support_roof_line_width.md) . Talán túl nagy a különbség a tartótető és a réteg többi szerkezete között. Lehet, hogy a vonal szélessége túl vékony a megfelelő extrudáláshoz. Ha a felületet [más anyaggal](../support/support_interface_extruder_nr.md) nyomtatják , gyakori probléma az, hogy az anyag, amelyre a felület nyomtatott, nem jut elegendő időhöz, hogy megfelelően elkezdjen folyni. Ez rögzíthető egy [primer torony](../dual/prime_tower_enable.md) használatával vagy [a tartótető területének](../support/support_roof_offset.md) növelésével.

Ha a támasz túl jól tapad a modellhez, a [vonalszélesség](../resolution/support_roof_line_width.md) beállítása általában hatékonyabb, mivel ez azt is eredményezi, hogy a vonalak közelebb kerülnek egymáshoz, hogy ugyanazt a támasztékkitöltési sűrűséget érjük el.
