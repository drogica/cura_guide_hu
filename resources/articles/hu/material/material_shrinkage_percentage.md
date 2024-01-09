# Méretezési tényező zsugorodási kompenzáció


<comment></comment>Ez a beállítás hatékonyan méretezi a modellt az automatikus szeletelés előtt. A cél az esetleges zsugorodás kompenzálása, amely akkor következik be, amikor a nyomat szobahőmérsékletre hűl. A kívántnál valamivel nagyobb nyomattal a végeredmény pontosabb lehet a bemeneti modell eredeti méreteihez képest. Ez a méretezési tényező minden dimenzióra (X, Y és Z) egyformán vonatkozik.

Az egész jelenet a középpontjától lesz méretezve. Ha több modellt nyomtat, akkor mindegyik ugyanarról a kiindulási pontról lesz méretezve. Ez lehetővé teszi, hogy ezeket a modelleket nagyon közel helyezze el egymáshoz anélkül, hogy a végső nyomatban átfednék őket. A modellek ütközési területei méretezve vannak, így pontosan láthatja, hová kerül a nyomat. Ez azt is megakadályozza, hogy a modelleket olyan helyeken helyezze el a jelenetben, ahol ütközhetnek a nyomat vagy a nyomtató jellemzőivel, például az alaptoronnyal vagy az építőlemez kapcsaival.

A 100%-os tényező nem okoz méretezést. A valamivel több, mint 100%-os méretezési tényező megfelelő számos mérnöki anyaghoz, mint például az ABS vagy a polipropilén. A 100%-nál kisebb méretezési tényező azt jelzi, hogy az anyag hűlés közben nő, mint egy hab.

A pusztán kémiai adatok arra vonatkozóan, hogy egy anyag mennyit zsugorodik a nyomtatási hőmérséklet és a szobahőmérséklet között, nem elegendőek ennek a beállításnak a jó értékének megjósolásához, mert a nyomtatási folyamat is befolyásolja a zsugorodást. Egy vonalban extrudálva a műanyag a vonal hosszának irányában megnyúlik, és ezen a tengelyen jobban zsugorodik. A zsugorodás nem egyenletes, de ez a beállítás csak egységes léptéktényezőt alkalmaz minden irányban. A pontos eredmények eléréséhez alkalmaznia kell a méretezési tényezőt az alkalmazás szempontjából legfontosabb tengelyen. Ha sok hosszú, egyenes vonal van a legfontosabb dimenzió mentén, akkor a méretezési tényezőnek nagyobbnak kell lennie.

Ha a méretezési tényező nagyobb, mint 100,5%, és valami nagyot nyomtat, akkor a Cura figyelmeztetést jelenít meg, hogy [vetemedést](../troubleshooting/warping.md) tapasztalhat.<!-- endif -->

<!--if cura_version < 4.8:This is a descriptive setting, letting Cura know how much the material shrinks when it cools down from the printing temperature to room temperature.

This setting is currently not used for slicing. It is currently only used to display a warning to the user when printing large things if the shrinkage ratio is larger than 0.5%.
-->

**Ez a beállítás nem látható a beállítások listájában. Ez csak egy belső beállítás, amelyet az anyagprofil felülír.**
