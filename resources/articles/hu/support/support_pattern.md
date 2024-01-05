# Támogatási minta

Ezzel a beállítással kiválaszthatja azt a mintát, amely a tartószerkezet térfogatának kitöltésére szolgál. A különböző mintáknak különböző erősségei és gyengeségei vannak.

<!--screenshot {
"image_path": "support_pattern_lines.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["rotateX(90)"]
    }
],
"camera_position": [0, 0, 135],
"settings": {
    "support_enable": true,
    "support_pattern": "lines"
},
"structures": ["helpers"],
"colours": 16
}-->

## Vonalak

![Vonalak](../images/support_pattern_lines.png)

A vonalminta egyenes vonalakat rajzol. A vonalak úgy vannak elhelyezve, hogy soha ne legyenek merőlegesek azokra a bőrvonalakra, amelyeket támogatnia kell (alapértelmezés szerint).

- A legkönnyebben eltávolítható az összes minta modelljéből. Ez nagyon hasznos, ha van egy túlnyúló terület, amely közel van az építőlemezhez. Szükség esetén késsel le lehet vágni a maradványokat.
- Az összes minta közül a legjobb túlnyúlási minőséget biztosítja a Cikcakkos technológiával együtt. A vonalak nagyon közel vannak egymáshoz, és úgy vannak elhelyezve, hogy ne legyenek merőlegesek a bőrre.
- Instabil, mivel a vonalak hajlamosak felborulni.

<!--screenshot {
"image_path": "support_pattern_grid.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["rotateX(90)"]
    }
],
"camera_position": [0, 0, 135],
"settings": {
    "support_enable": true,
    "support_pattern": "grid"
},
"structures": ["helpers"],
"colours": 16
}-->

## Rács

![Rács](../images/support_pattern_grid.png)

A rácsminta két egymásra merőleges egyenest rajzol. Átfedik egymást, négyzetmintát alkotva. Alapértelmezés szerint a rendszer egy kerületet rajzol a minta köré.

- Nagyon erős, megbízhatóan növekszik.
- Közepes túlnyúlási minőséget biztosít, mivel a vonalak meglehetősen távol vannak egymástól.
- Nehéz eltávolítani, mivel a támaszték nem nagyon hajlik.

<!--screenshot {
"image_path": "support_pattern_triangles.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["rotateX(90)"]
    }
],
"camera_position": [0, 0, 135],
"settings": {
    "support_enable": true,
    "support_pattern": "triangles"
},
"structures": ["helpers"],
"colours": 16
}-->

## Háromszögek

![Háromszögek](../images/support_pattern_triangles.png)

A háromszög minta három sor egyenes vonalat rajzol egymással 60 fokos szögben, egyenlő oldalú háromszögek mintáját alkotva. Alapértelmezés szerint a rendszer egy kerületet rajzol a minta köré.

- Az összes támasztóminta közül a legerősebb.
- Rossz túlnyúlási minőséget biztosít, mivel a vonalak nagyon távol vannak egymástól.
- Nehéz lehet eltávolítani, mivel a támaszték egyáltalán nem hajlik meg semmilyen irányba.

<!--screenshot {
"image_path": "support_pattern_concentric.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["rotateX(90)"]
    }
],
"camera_position": [0, 0, 135],
"settings": {
    "support_enable": true,
    "support_pattern": "concentric"
},
"structures": ["helpers"],
"colours": 16
}-->

## Körkörös

![Körkörös](../images/support_pattern_concentric.png)

A koncentrikus mintázat következtében a támaszték koncentrikus gyűrűkből áll, amelyek kívülről befelé egyenletesen helyezkednek el.

- A vonalak közel vannak egymáshoz, így jó alátámasztást biztosítanak a túlnyúlásoknak a sima felület érdekében, ha a vonalak merőlegesek.
- Meglehetősen masszív, mivel a hurkok külön-külön is nagy szélességben állhatnak.
- Könnyen eltávolítható, mivel a tartószerkezet könnyen befelé hajlik.
- Gyakran párhuzamosan végződik a falakkal, amelyeket támogatnia kell. Ez rosszabb túlnyúlási minőséget eredményez, mivel egyes falak egyáltalán nem kapnak alátámasztást.
- Néha a támogatás felfüggesztéséhez vezet a levegőben.

<!--screenshot {
"image_path": "support_pattern_zigzag.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["rotateX(90)"]
    }
],
"camera_position": [0, 0, 135],
"settings": {
    "support_enable": true,
    "support_pattern": "zigzag"
},
"structures": ["helpers"],
"colours": 16
}-->

## Cikcakk

![Cikcakk](../images/support_pattern_zigzag.png)

A cikk-cakk minta olyan, mint a vonalminta, de a vonalak a végeken össze vannak kötve.

- Meglehetősen masszív, nagymértékben növeli a megbízhatóságot.
- A vonalakkal együtt minden minta közül a legjobb túlnyúlási minőséget biztosítja. A vonalak nagyon közel vannak egymáshoz, és úgy vannak elhelyezve, hogy ne legyenek merőlegesek a bőrre.
- Könnyen eltávolítható. A tartószerkezet befelé hajlik, ráhúzáskor a támasz csíkokban húzódik le.
- Szinte mindig egyetlen vonalba húzza a támasztékot, minimálisra csökkentve a visszahúzások vagy az utazási mozdulatok szükségességét.

<!--screenshot {
"image_path": "support_pattern_cross.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["rotateX(90)"]
    }
],
"camera_position": [0, 0, 135],
"settings": {
    "support_enable": true,
    "support_pattern": "cross"
},
"structures": ["helpers"],
"colours": 16
}-->

## Kereszt

![Kereszt](../images/support_pattern_cross.png)

A keresztminta töredékmintát rajzol az egész kötetre, benne keresztszerű alakzatokkal.

- Az összes minta közül a legkönnyebben hajlítható, mivel ebben a mintában nincsenek hosszú egyenes vonalak.
- Szinte mindig egyetlen vonalba húzza a támasztékot, minimálisra csökkentve a visszahúzások vagy az utazási mozgások szükségességét.

<!--screenshot {
"image_path": "support_pattern_gyroid.png",
"models": [
    {
        "script": "calendar_holder.scad",
        "transformation": ["rotateX(90)"]
    }
],
"camera_position": [0, 0, 135],
"settings": {
    "support_enable": true,
    "support_pattern": "gyroid"
},
"structures": ["helpers"],
"colours": 16
}-->

<!--if cura_version >= 4.1-->

## Gyroid

![Gyroid](../images/support_pattern_gyroid.png)

A gyroid mintája hullámos, görbe előre-hátra billeg. A görbe rétegenként változik.

- Meglehetősen masszív minta, növeli a megbízhatóságot.
- A tartó közötti levegő egyetlen térfogat. Oldható hordozóanyagokkal történő nyomtatás esetén ez lehetővé teszi, hogy az oldószer (víz, etanol vagy egyéb) a tartószerkezet minden belső részébe kinyúljon, még akkor is, ha van alatta perem. Ez lehetővé teszi a támasz gyorsabb feloldását.
- A túlnyúlás minden vonalát egyenletesen támogatja, azok irányától függetlenül.

<!--endif-->
