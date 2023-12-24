# Forma szög

A [Túlnyúlás nyomtathatóvá tétele](../experimental/conical_overhang_enabled.md) funkcióhoz hasonlóan ez a beállítás módosítja a formák alakját, hogy támogatás nélkül is ki lehessen nyomtatni. Csak a forma külső formája módosul, így az öntvény alakja nem változik.

<!--screenshot {
"image_path": "mold_angle.png",
"models": [
    {
        "script": "star_podium.scad",
        "transformation": ["mirrorZ"]
    }
],
"camera_position": [81, 129, 45],
"settings": {
    "mold_enabled": "True"
},
"colours": 48
}-->

![A 40 fokos szög lehetővé teszi a forma alsó oldalának nyomtatását anélkül, hogy szükség lenne rá](../images/mold_angle.png)

Ennek a szögnek a csökkentése csökkenti a túlnyúlások végét. Ez megbízhatóbbá teszi a nyomtatást. Ugyanakkor szélesebbé teszi a nyomat alapját, ami jelentősen megnöveli a nyomat időtartamát és növeli a felhasznált anyag mennyiségét.

Egyes formák esetében a forma külső alakjának módosítása nem elegendő a megfelelő nyomtatáshoz. Még mindig támogatásra lesz szüksége. Hasonló hatást érhet el [a Conical Support](../support/support_conical_enabled.md) engedélyezésével.

<!--screenshot {
"image_path": "mold_needs_support.png",
"models": [{"script": "basic_overhang.scad"}],
"camera_position": [20, 183, 97],
"settings": {
    "mold_enabled": "True"
},
"colours": 32
}-->

![Ennek a formának még támogatásra van szüksége](../images/mold_needs_support.png)
