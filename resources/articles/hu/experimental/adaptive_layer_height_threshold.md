# Adaptív rétegek domborzati mérete

Ez a beállítás konfigurálja, hogy a fóliák határai milyen távolságra (vízszintesen) legyenek elhelyezve bármely lejtőn. A réteg magasságát úgy állítjuk be, hogy a kívánt elmozdulást elérjük. Amikor megpróbálja megakadályozni a [topográfiai hatást](../troubleshooting/topography.md) , ez a beállítás lényegében azt konfigurálja, hogy a topográfiai kontúrok milyen távolságra legyenek egymástól.

Ennek a beállításnak a csökkentésével a rétegek összességében vékonyabbak lesznek, mert a rétegek vízszintes széleit közelebb kell egymáshoz helyezni. A beállítás növelésével a rétegek vastagabbak lesznek, mert a rétegek szélei távolabb helyezkedhetnek el egymástól. A rétegek vastagsága azonban a [Rétegmagasság](../resolution/layer_height.md) és [Variáció](adaptive_layer_height_variation.md) beállítások által meghatározott tartományon belül marad.

Csökkentse ezt a beállítást, hogy csökkentse a topográfiai hatást a nyomat felső vagy alsó oldalán. Ennek ellenére a nyomtatás tovább tart. Növelje ezt a beállítást a nyomtatási idő csökkentéséhez.

Szinte mindig jobb a Layer Height beállítást módosítani e beállítás helyett, és ennek megfelelően módosítani a többi beállítást. Kezdje egy olyan profillal, amelynek rétegmagassága szükséges ahhoz, hogy a domborzati hatást elfogadható szintre csökkentse. Ezután engedjen némi eltérést a rétegvastagság körül az adaptív rétegekkel. Ez biztosítja, hogy a többi nyomtatási beállítás megfelelően legyen beállítva a ténylegesen nyomtatandó rétegvastagsághoz. Ezzel a beállítással enyhén súlyozhatja az adaptív rétegeket, hogy többet válasszon a megengedett tartomány alsó vagy felső részéből.
