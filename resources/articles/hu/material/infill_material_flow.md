# Kitöltési áramlás

Ez a beállítás csak a feltöltéshez állítja be az áramlási sebességet. A kitöltés áramlási sebessége a nyomat többi részének áramlási sebességétől külön állítható.

Az áramlási sebesség beállítása a feltöltés során az extrudálási sebességgel vagy szilárdsággal kapcsolatos problémák megoldására szolgáló ütközőrés módszer. Ugyanez a hatás érhető el a vonalak [közötti távolság](../infill/infill_line_distance.md) és a kitöltés [vonalszélességének](../resolution/infill_line_width.md) beállításával, de ez a beállítás intuitívabb lehet.

Az extrudálási sebességgel vagy a kitöltés szilárdságával kapcsolatos problémákat jellemzően két dolog egyike okozza: a kitöltési minta keresztezései, vagy az áramlási sebesség túl nagy változása a kitöltés és más szerkezetek között. Ahelyett, hogy ezt az áramlási sebességet módosítaná, hatékonyabb lehet a [kitöltési minta](../infill/infill_pattern.md) vagy a [vonalszélesség](../resolution/infill_line_width.md) beállítása. Válasszon olyan kitöltési mintát, amely nem keresztezi önmagát, például cikk-cakk, és válasszon olyan vonalszélességet, amely közelebb áll a falak és a burkolat extrudálási sebességéhez. Ha a vonal szélességét növelni kell a szilárdság érdekében, de az áramlási sebesség korlátozott, akkor az áramlás növelése helyett érdemes a [kitöltési szorzót](../infill/infill_multiplier.md) használni.
