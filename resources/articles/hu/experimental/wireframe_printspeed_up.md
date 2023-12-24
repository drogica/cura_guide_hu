# WP felfelé irányuló nyomtatási sebesség

Ez a beállítás megadja, hogy a fúvóka milyen gyorsan mozogjon felfelé, miközben függőleges mozgást végez a fűrészfog mintázatában. A felfelé mozgás sebessége a többi drótnyomtatási sebességtől külön konfigurálható.

![Ahol a különböző vezetékes nyomtatási sebességek érvényesek](../images/wireframe_printspeed.svg)

A felfelé irányuló mozgás nem lesz a megadott sebességű a teljes mozgás során. Az [Ease Upward](wireframe_up_half_speed.md) beállítás által meghatározott felfelé irányuló mozgás legalacsonyabb bitjénél a nyomtatófej ennek a sebességnek a felével fog mozogni.

Ha lassabban halad felfelé, az több időt vesz igénybe, de több időt hagy az anyagnak megszilárdulni. Így nem húzódik annyira magával az átló irányába. Azonban a túl lassú mozgás a vezetéket is lefelé nyomja az izzószál tehetetlensége miatt a fúvókakamrában lévő nyomással. Ekkor az izzószál hajlamos inogni, ami kevésbé valószínű, hogy a következő vízszintes vonal megfelelő kapcsolatot tud létrehozni.
