# Fúvóka átmérője

Ez a beállítás annak a fúvókanyílásnak az átmérőjét méri, amelyen keresztül az anyag átfolyik.

![A nyomtatófej méretei](../images/head_dimensions.svg)

Ez egy fontos dimenzió, amelyre más beállítások alapozhatják az alapértelmezett értékeket. A legfontosabb, hogy a [vonalszélességet](../resolution/line_width.md) általában a fúvóka méretétől függően állítják be. Egyes nyomtatóprofilok a fúvóka mérete alapján is korlátozzák a rétegmagasságot, mivel a fúvóka mérete a legfontosabb tényező az anyag extrudálhatóságában.

<!--if cura_version < 5.0:The nozzle size is also used directly, for one detail: When filling [tiny gaps](../shell/fill_perimeter_gaps.md), line pieces further than two nozzle sizes away from each other are not merged together.-->

Ne módosítsa a fúvóka méretét, hacsak nem módosítja a fizikai fúvókát. Egyes szeletelők (beleértve a Cura 15.04-et és korábbi verziókat is) a "fúvókaméret" kifejezést használják arra vonatkozóan, hogy milyen szélesnek kell lenniük a nyomat vonalainak. A Cura ehhez a [Vonalszélesség](../resolution/line_width.md) beállítást használja.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában. Ha a nyomtatója speciális profilokkal rendelkezik a rendelkezésre álló fúvókákhoz, ezek közül választhat a képernyő felső, középső részén található nyomtatóbeállítási menüben. Ellenkező esetben a fúvóka átmérőjét a nyomtatóbeállítások párbeszédpanelen állíthatja be, amely a beállítások párbeszédpanel hozzáadott nyomtatóinak listájában található.**
