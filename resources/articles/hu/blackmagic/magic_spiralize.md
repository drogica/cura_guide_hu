# Spiralizálja a külső kontúrt

A Spiralize Outer Contour egy trükk.

Rétegenkénti nyomtatáskor a fúvókának általában egyik rétegről a másikra kell mozognia. Ez a mozgás hatására a fúvóka a másodperc töredékéig szinte mozdulatlanul áll, ami egy varratot hagy a felületen, az úgynevezett Z varrat. Ez a beállítás ennek és még sok másnak a megakadályozására szolgál. Nagyban leegyszerűsíti a nyomtatási folyamatot azáltal, hogy sok szempontot kihagy belőle.

A modell spirálozása során a modell nem kap kitöltést vagy felsőket. Csak egy falat és egy aljat kap. Lényeges, hogy ha [a Smooth Spiralized Contours](smooth_spiralized_contours.md) engedélyezve van, a fúvóka magassága fokozatosan növekszik a réteg során. Így a modell kontúrját követve spirál jön létre. Nem lesz mozgás egyik rétegről a másikra, mert a fúvóka már fokozatosan a következő réteg felé mozdult.

A spiralizálási mód sok szeletelőnél gyakori. Néha "váza módnak" is nevezik, mert ez egy jó módja a vázák nyomtatásának. Néhány egyéb tulajdonság a következőket tartalmazza:

- Rendkívül gyorsan nyomtat.
- A felület nagyon sima lesz. Ha [a Smooth Spiralized Contours](smooth_spiralized_contours.md) engedélyezve van, már nincs [Z-varrás](../troubleshooting/seam.md) , ahol a következő rétegre került.
- Nem lesz túl erős. Ha a modell túl nagy, a vékony fal miatt hajlamos [széthasadni](../troubleshooting/layer_splitting.md) .
- Míg a varrás eltávolítása segít a nyomat vízállóvá tételében, nehéz a nyomatot vízállóvá tenni, ha bármilyen mérete van. Ehhez ajánlatos legalább 2 falat. A külső kontúr spiralizálása ekkor lehetetlen.

**A spiralizálás nem működik jól sok vízszintes felületet tartalmazó nyomatoknál. Egyáltalán nem kezeli a túlnyúlásokat, és nem nyomtatja a felső felületeket, így semmi sem dőlhet vízszintes felületre. Akkor sem működik jól, ha több rész van egy rétegen.**
