# Gantry magasság

Ez a beállítás méri a távolságot az alaplap és a portálrendszer között, amelyre a nyomtatófej fel van függesztve. Ez a magasság egy mennyezetet jelent, amikor [egyszerre csak egy objektumot](../blackmagic/print_sequence.md) nyomtat, mivel a korábban kinyomtatott objektumok a portálnak ütközhetnek.

![A nyomtatófej méretei](../images/head_dimensions.svg)

A legtöbb 3D nyomtató nyomtatófeje egy-két keresztrúdon lóg. Ennek a portálnak a formáját nem Cura modellezte: legyen szó két keresztező rúdról, egyetlen irányból bejövő karról vagy egyetlen keresztrúdról, amely mentén a nyomtatófej egy irányba mozoghat. Cura ezt az állványt kemény mennyezetnek tekinti, amikor egyesével nyomtat, függetlenül attól, hogy a modelleket milyen sorrendben nyomtatják. Egyenkénti nyomtatáskor a felépítési térfogat magassága erre a portálmagasságra csökken, jelezve, hogy nincsenek modellek. a portálmagasságnál magasabbak megengedettek.

Egy kivétel az, amikor csak egy objektum van betöltve az építőlemezre. Ez az objektum magasabb lehet, mint a portál magassága, mivel semmi más nem lesz az építőlemezen, ami ekkor ütközhetne a portálral.

**Mivel ez egy gépbeállítás, általában nem jelenik meg a normál beállítások listájában. A portál magassága a nyomtatóbeállítások párbeszédpanelen módosítható, amely a beállítások párbeszédablakban található hozzáadott nyomtatók listájában található.**
