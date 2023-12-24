# Maximális túlnyúló furat terület

Mivel [a Make Overhang Printable](conical_overhang_enabled.md) eltávolít mindenféle túlnyúlást, minden híd automatikusan leereszkedik, lezárva az alatta lévő túlnyúlást. Ha azonban a túlnyúlás minden oldalról be van zárva, akkor folyamatosan süllyed, amíg a zárt túlnyúlás teljesen fel nem telik. Valójában minden lefelé néző lyuk teljesen feltöltődik, még akkor is, ha az eltávolítandó túlnyúlás csak egy apró folt a legfelül.

Ennek a hatásnak a megelőzése érdekében ez a beállítás lehetővé teszi, hogy a túlnyúlás nyitva maradjon, ha minden oldalról be van zárva, és kisebb, mint egy bizonyos terület. Ez csak a lyukakra vonatkozik. A modell külső részének szabályos túlnyúlása továbbra is lefelé van meghosszabbítva, hogy megőrizze az ésszerűen nyomtatható szöget.

<!--screenshot {
"image_path": "conical_overhang_hole_size.png",
"models": [{"script": "plopper.scad"}],
"camera_position": [-86, 29, -85],
"settings": {
    "conical_overhang_enabled": true,
    "conical_overhang_hole_size": 20
},
"colours": 64
}-->

![A tetején egy kis hely kilóghat, így ez a lyuk nem tömődik be](../images/conical_overhang_hole_size.png)

Meglehetősen biztonságos ezt a beállítást több tucat négyzetmilliméterre állítani a legtöbb modellnél. Ha túl alacsonyra van állítva, a modell többet módosítani fog, hogy támogassa azokat a túlnyúlásokat, amelyek valóban túl kicsik ahhoz, hogy támogatásra szoruljanak. Ha azonban túl magasra van állítva, jelentős túlnyúló területek lesznek, amelyeket nehéz áthidalni.

Ha ennek a beállításnak köszönhetően nagy a túlnyúlás, érdemes először megvizsgálni [az áthidalás hangolását](bridge_settings_enabled.md) , mielőtt megpróbálná módosítani a modellt a túlnyúlás eltávolítása érdekében.
