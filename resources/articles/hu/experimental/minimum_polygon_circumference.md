# Minimális sokszög kerülete

A Cura általában eltávolítja a modell azon részleteit, amelyek kisebbek, mint amennyit a fúvóka ki tud nyomtatni. Ezzel a beállítással módosíthatja ezt a küszöböt több vagy kevesebb részlet eltávolításához. Ez a beállítás minden rétegen minden alakzat kerületét méri, és ha az kisebb, mint ennek a beállításnak az értéke, akkor az alakzat nem kerül nyomtatásra.

Jó ötlet az egy vonalszélességnél kisebb részletek eltávolítása. Ez kissé felgyorsítja a szeletelést. Ez azonban nem mindig igaz azokra az alkatrészekre, amelyek kisebbek, mint a [külső fal vonalszélessége](../resolution/wall_line_width_0.md) , ha a [Vékony falak nyomtatása](../shell/fill_outline_gaps.md) funkció engedélyezve van. Ha még mindig nagyon kicsi darabokat kell megkísérelni, akkor ezt a beállítást kisebbre állíthatja.

A beállítás növelése segíthet az apró részletek eltávolításában és gyorsabb nyomtatásban. Ha nem kell kinyomtatnia ezeket az apró részleteket, megspórolhat néhány utazást, hogy elérje őket.
