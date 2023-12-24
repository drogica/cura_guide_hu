# Drótnyomtatás

Ez a beállítás egy teljesen más nyomtatási módot tesz lehetővé, úgynevezett Wire Printing. Drótnyomtatás használatakor a nyomtató nem tömör tárgyat, hanem csak egy külső alakú háromszöghálót készít vékony huzalokból.

Ennek a technikának számos előnye van:

- Sokkal gyorsabban nyomtat, mint egy tömör tárgy.
- Csak töredékét használja fel a normál nyomtatáshoz használt anyagnak.
- Különlegesnek tűnik, mintha kézzel készítették volna 3D nyomtatótollal.

A kapott objektum azonban nem működik. Nagyjából a megfelelő méretű lesz, ami hasznossá teszi a nyomat méretarányának prototípusának elkészítéséhez, bár a méret sem lesz túl pontos. Az így kapott tárgy rendkívül sérülékeny, nemcsak nyomtatás közben, hanem utána is. Nehéz leszedni az építőlemezről anélkül, hogy megsérülne. A modell részletének nagy részét is elveszíti.

A drótnyomtatás meglehetősen széles, több milliméteres függőleges távolságú anyaggyűrűk lerakásával működik. Ezek közé a gyűrűk közé fűrészfog alakot rajzol, amely lehetővé teszi, hogy a következő gyűrű az előző tetején feküdjön. Ahol a modell felülete vízszintesre megy, hasonló technikát alkalmaznak a tetejének lezárására. A tetőben koncentrikus gyűrűk találhatók, amelyeket fűrészfog-forma tart össze, amelyeket kívülről (ahol falon tud támaszkodni) befelé építve óvatosan a levegőben felfüggeszteni.

A drótnyomtatás csak akkor működik igazán megbízhatóan, ha a formák szinte teljesen függőlegesek, hasonlóan ahhoz a típushoz, amely jól működik [a Spiralize Mode](../blackmagic/magic_spiralize.md) esetén. Ha a felület nagy területen vízszintes, akkor a tetőzárási technikának rendkívül nagy távolságot kell áthidalnia. Ez akkor nagy valószínűséggel sikertelen lesz. Ha a modell ezután felfelé halad a vízszintes felület felénél, akkor szinte biztos, hogy a levegőben nyomtatják.

**A Cura rétegnézete nem jeleníti meg megfelelően a vezetékes nyomtatást közvetlenül a szeletelés után. Az eredmény azonban továbbra is megtekinthető, ha elmenti a g-kódot a lemezre, és újra megnyitja a g-kódot a Curával.**
