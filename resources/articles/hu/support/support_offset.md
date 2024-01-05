# Támogatja a vízszintes terjeszkedést

Ez a beállítás azt eredményezi, hogy a támaszték kissé szélesebbé válik, és vízszintesen kitágul minden irányba.

<!--screenshot {
"image_path": "support_offset.png",
"models": [{"script": "duct.scad"}],
"camera_position": [47, 72, 128],
"settings": {
    "support_enable": true,
    "support_offset": 1.6
},
"colours": 64
}-->

![A támogatás szélesebb a modell támogatásához szükségesnél](../images/support_offset.png)

Ez a beállítás többféleképpen használható a támogatáshoz használt anyagtól és a támogatásra szoruló modell típusától függően:

- Ennek a beállításnak a növelése szélesebbé és ezáltal szilárdabbá teszi a támogatást. Ez a kis túlnyúlású magas modelleknél hasznos, mivel a túlnyúlást egyébként egy nagyon magas, vékony tartóoszlop támasztja alá. Némi vízszintes bővítéssel nagyon magas, de kissé szélesebb támasztóoszlop lesz.
- A beállítás növelése biztonsági intézkedésként is funkcionál annak biztosítására, hogy a támasztóterületek rendelkezzenek egy bizonyos minimális területtel. Ez a nehezen extrudálható anyagok, például a PVA esetében szükséges.
- A beállítás csökkentése csökkenti az anyagfelhasználást és a támogatáshoz szükséges nyomtatási időt. Ennek növelése természetesen növeli a szükséges anyag- és nyomtatási időt. Lásd még a [kúpos támasztó](support_conical_enabled.md) funkciót, amely csökkenti a támaszték szélességét anélkül, hogy veszélyeztetné a támaszték által megtámasztott területet.
- Ha ezt a beállítást negatív értékre állítja, akkor a vékony támasztóoszlopokat is teljesen eltávolíthatja. Ha ez a támogatás úgysem sikerülne kinyomtatni, jobb lehet, ha teljesen elhagyja. A támogatás blokkoló eszköze egy módszer a támogatás eltávolítására anélkül, hogy veszélyeztetné a modell többi részének túlnyúlását.
