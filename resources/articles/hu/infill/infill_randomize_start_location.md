# Véletlenszerű kitöltés kezdete

Ha ez a beállítás engedélyezve van, a nyomtató véletlenszerűen kiválasztja azt a pozíciót, ahol a nyomtató elkezdi a kitöltés nyomtatását egy rétegre.

A kitöltő pálya eleje általában valamivel gyengébb, mint a kitöltés többi része. Ez akkor fordul elő, ha a kitöltés gyorsabban, vastagabb vonalakkal vagy nagyobb rétegmagassággal kerül nyomtatásra. Az anyagáramlásnak hirtelen fel kell gyorsulnia, és ez nem történik meg azonnal, így rövid ideig alulextrudálás következik be. Ha ez minden rétegben ugyanazon a helyen történik, az gyengíti a kitöltési struktúrát. Az a hely, ahol ez megtörténik, lesz a leggyengébb láncszem, és a körülötte lévő kitöltés nagyobb igénybevételnek lesz kitéve. Ha a nyomatot erőnek teszik ki, itt nagyobb a valószínűsége, hogy eltörik.

Normális esetben a feltöltés azzal a vonallal kezdődik, amely a legközelebb van ahhoz a pozícióhoz, ahol a fúvóka volt, amikor a feltöltéssel kezdődik, hogy csökkentse az utazási időt. Ha ez a beállítás engedélyezve van, akkor a kiindulási hely véletlenszerű lesz. Ez szétteríti a gyenge pontokat. Egyetlen leggyengébb láncszem sem lesz többé a láncban, így a kitöltés is erősebb lesz a végén.

Ez azonban kissé megnöveli az utazási időt, és több szivárgást eredményez a modell belsejében, mivel a kitöltés kiindulási helyétől való távolság már nincs minimálisra csökkentve.

**Bár a kiindulási hely véletlenszerűen van elosztva, még mindig determinisztikus. Ugyanazon szelet kétszeri megismétlése ugyanazokat a kiindulási helyeket eredményezi.**
