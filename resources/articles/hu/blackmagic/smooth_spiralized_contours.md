# Sima spiralizált kontúrok

Ha [a Spiralizálás](magic_spiralize.md) engedélyezve van, ez a beállítás engedélyezi vagy letiltja a Spiralizálás mód legjellemzőbb jellemzőjét: Ahelyett, hogy az egyes rétegeket egymás után, magassági időközönként nyomtatná ki, a magasság fokozatosan nő a réteg során.

Mivel a Spiralize mód csak a falakat nyomtatja a legtöbb rétegre egyetlen kontúrral, ez az egyetlen kontúr spirál formáját ölti, ami a Spiralize funkció nevét adja. A nyomat első és utolsó rétegének áramlási sebessége fokozatosan csökken a túlextrudálás megelőzése és a megfelelő magasság elérése érdekében.

Mivel a fúvókát fokozatosan a következő rétegmagasságig mozgatják az egész rétegben, többé nem lesz olyan varrat, ahol a fúvóka a következő rétegre kerül. Ez hatékonyan eltávolítja a Z varratot.

Másrészt a réteg felfelé vagy lefelé mozog fél rétegmagassággal. Ez kevésbé pontos. Elmosódó hatást gyakorolhat a nyomat finom részleteire.

Ez a beállítás nem hatékony a varratok eltávolítására, ha egy rétegre több kontúrt kell nyomtatni. A kontúr után továbbra is le kell állítania az extrudálást, hogy a következő nyomtatott darabra léphessen. Ettől amúgy is varrás marad.

**Ez a hatás nem látható rétegnézetben a megjelenítési korlátok miatt.**
