# Tedd nyomtathatóvá a túlnyúlást

Ez a beállítás úgy alakítja át a modellt, hogy többé ne legyen túlnyúlása. Extra anyagot helyez el minden túlnyúlás alá, és úgy nyomtatja ki, mintha a modell része lenne.

<!--screenshot {
"image_path": "conical_overhang_enabled_disabled.png",
"models": [{"script": "castle.scad"}],
"camera_position": [0, 189, 25],
"settings": {
    "conical_overhang_enabled": false
},
"colours": 8
}-->

<!--screenshot {
"image_path": "conical_overhang_enabled_enabled.png",
"models": [{"script": "castle.scad"}],
"camera_position": [0, 189, 25],
"settings": {
    "conical_overhang_enabled": true,
    "conical_overhang_angle": 50
},
"colours": 8
}-->

![Egy torony néhány kilógó darabbal](../images/conical_overhang_enabled_disabled.png)![A túlnyúlás nyomtatható](../images/conical_overhang_enabled_enabled.png)

Az összes kilógó darab alá valamilyen anyagot helyeznek el, amely lefelé fokozatosan csökken. Sok esetben a túlnyúlás maga a tárgy felé dől. A lejtést, amelynél a túlnyúlás az objektum felé nő, a [modellszög](conical_overhang_angle.md) határozza meg.

Ez a beállítás egyszerű módja lehet annak, hogy ne legyen szükség támogatásra. Különösen hatásos, ha kissé érdes felületű vagy oldalsó domborművel rendelkező modelleket nyomtat. Ezek a kis túlnyúlások általában leereszkednek, és szétkapcsolt műanyag húrok laza szálait képezik. Lehetséges, hogy bizonyos támogatással támogatják őket, de ez költséges lehet a nyomtatási idő tekintetében, és így is hagy némi hegesedést. Ha ez a beállítás engedélyezve van, a túlnyúlás a modell felé simítva lesz. Úgy fog tűnni, mintha így akarták volna kinyomtatni.

Ha a túlnyúlás messzebbre nyúlik ki a fő testből, mint a szélessége, ez még mindig eredményezhet némi túlnyúlást vonal formájában. Ez azért történik, mert a kiemelkedés végtelenül vékonyra zsugorodik, amitől eltűnik. Ha ez megtörténik, mérlegelheti, hogy szükség lehet-e továbbra is a támogatás nyomtatására. A fenti képek esetében ez a torony oldalán lévő kis tömböknél történik, de olyan kicsik, hogy az egyszerű áthidalás valószínűleg lehetővé teszi, hogy jól lelógjon.
