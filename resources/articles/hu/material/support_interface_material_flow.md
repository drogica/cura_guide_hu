# Interfész Flow támogatása

Ez a beállítás csak a támogatási interfész áramlási sebességét állítja be. A támasztó interfész áramlási sebessége a tartó többi részének áramlási sebességétől külön állítható.

Az áramlási sebesség beállítása a támasztó interfész alatt egy ütközőrés módszer az extrudálási sebességgel vagy a modell és a támaszték közötti tapadással kapcsolatos problémák megoldására. Ugyanez a hatás érhető el a támasztófelület [vonalszélességének](../resolution/support_interface_line_width.md) vagy [sortávolságának](../support/support_roof_line_distance.md) beállításával, de az áramlási sebesség beállítása intuitívabb lehet.

Ha probléma van az extrudálási sebességgel, jobb, ha megnézi a [nyomtatási sebességet](../speed/speed_support_interface.md) , [a hőmérsékletet](material_print_temperature.md) és [a vonalszélességet](../resolution/support_interface_line_width.md) . Talán túl nagy a különbség a hordozó interfész áramlási sebessége és a réteg többi struktúrája között. Lehet, hogy a vonal szélessége túl vékony a megfelelő extrudáláshoz. Ha a felületet [más anyaggal](../support/support_interface_extruder_nr.md) nyomtatják , gyakori probléma az, hogy az anyag, amelyre a felület nyomtatott, nem jut elegendő időhöz, hogy megfelelően elkezdjen folyni. Ez javítható egy [prime torony](../dual/prime_tower_enable.md) használatával vagy [a támasztó interfész területének](../support/support_interface_offset.md) növelésével.

Ha a támasz túl jól tapad a modellhez, a [vonalszélesség](../resolution/support_interface_line_width.md) beállítása általában hatékonyabb, mivel ez azt is eredményezi, hogy a vonalak közelebb kerülnek egymáshoz, hogy ugyanazt a támasztékkitöltési sűrűséget érjük el.
