# Szakítási támogatás darabokban

Ha cikkcakkos [mintát](../support/support_pattern.md) használunk a támasztékhoz, a támaszt össze lehet gyűrni, így könnyen eltávolítható. Ez nehezebbé válik, ha a támaszték nagyon széles. Ezzel a beállítással a cikk-cakk támaszték olyan darabokra oszlik, amelyek egyenként könnyebben letörhetők, de még mindig elég szélesek ahhoz, hogy megőrizzék stabilitásukat.

<!--screenshot {
"image_path": "support_skip_some_zags.png",
"models": [{"script": "rack.scad"}],
"camera_position": [0, 184, 10],
"settings": {
    "support_enable": true,
    "support_pattern": "zigzag",
    "support_skip_some_zags": true,
    "support_skip_zag_per_mm": 20
},
"colours": 32
}-->

![8 soronként kimarad egy összekötő vonal, amely darabokra bontja a támasztékot](../images/support_skip_some_zags.png)

A támaszték darabokra bontása megkönnyíti a támaszték letörését, mert a támasztékot egyenként is letörheti. Ez azonban kissé csökkenti a támaszték szilárdságát és merevségét, különösen, ha a [darab mérete](support_skip_zag_per_mm.md) nagyon kicsi. Ennek eredményeként valamivel nagyobb az esélye annak, hogy a támasz felborul, ami sok húrozást és rossz túlnyúlásokat eredményez.

Ez a beállítás azt is megakadályozza, hogy az összes támaszt egy darabban húzza le. Ha sok a tartóelem, azokat egyenként kell levenni. Ha egyébként a támasz elég könnyen leválik, akkor ez a beállítás valóban megnövelheti a támasz lehúzását (bár lehet, hogy így is könnyebb).

Ez a beállítás nem jól kombinálható [a Support Wall Line Count](../support/support_wall_count.md) funkcióval. Ha a tartón van egy extra fal körülötte, ez a fal ismét összeköti a darabokat, megnehezítve a darabok letörését.
