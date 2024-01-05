# Minimális támogatási terület

Ez a beállítás minimális megengedett méretet ír elő a támasztékdarabokhoz. Ha egy támasztéknak kisebb területe van, mint ennek a beállításnak az értéke egy bizonyos rétegen, akkor a támasz kimarad.

<!--screenshot {
"image_path": "minimum_support_area_0.png",
"models": [{"script": "castle.scad"}],
"camera_position": [0, 190, 47],
"settings": {
    "support_enable": true,
    "minimum_support_area": 0
},
"colours": 64
}-->

<!--screenshot {
"image_path": "minimum_support_area_10.png",
"models": [{"script": "castle.scad"}],
"camera_position": [0, 190, 47],
"settings": {
    "support_enable": true,
    "minimum_support_area": 10
},
"colours": 64
}-->

![Nincs terület szűrése (a minimális terület 0)](../images/minimum_support_area_0.png)![A kis támasztékdarabok kimaradnak](../images/minimum_support_area_10.png)

Ez a beállítás azért létezik, mert a vékony támasztóoszlopok valószínűleg felborulnak. Általában támogatják a kis funkciókat is, amelyek támogatás nélkül valószínűleg jól nyomtatnának. Ha a támasz felborul, sok folt marad a nyomaton. Ezért jobb lehet elhagyni ezeket a vékony oszlopokat. Ez a beállítás lehetőséget biztosít a támaszték kiszűrésére az oszlop keresztmetszete alapján.

A terület növelése csökkenti a nyomtatott támaszték mennyiségét, enyhén csökkentve az időt és az anyagfelhasználást. Ennél is fontosabb, hogy javítja a nyomat megbízhatóságát, mivel kisebb az esélye a tartóoszlopok felborulásának. Ugyanakkor a nyomat kis jellemzőinek támogatását is megszünteti, így a túlnyúlás minősége romolhat ezeknél a daraboknál.

Egyes alakzatoknál ez azzal a kellemetlen mellékhatással járhat, hogy eltávolítja a támaszték felső részét, ha a felső rész a küszöb alá esik, de az alsó rész nem. Emiatt előfordulhat, hogy azok az alkatrészek nem támogatottak, amelyekre általában számítana.

<!--screenshot {
"image_path": "minimum_support_area_problem.png",
"models": [{"script": "overhang_bridging_cooling.scad"}],
"camera_position": [117, 0, 15],
"settings": {
    "support_enable": true,
    "minimum_support_area": 50
},
"colours": 64
}-->

![Az ív csúcsa nem támogatott, mert ezeken a rétegeken túl kicsi a terület](../images/minimum_support_area_problem.png)
