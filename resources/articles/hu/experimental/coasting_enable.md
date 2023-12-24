# Coasting engedélyezése

Ha ez a beállítás engedélyezve van, a fúvóka kissé leállítja az anyag extrudálását, mielőtt lezárná a fal kontúrját. Az ötlet az, hogy a fúvóka kamra az utolsó vonalon kiürítheti magát, ami csökkenti a fúvókára nehezedő nyomást, és lehetővé teszi, hogy a kontúr kezdete előtt blokkolja azt. Így kevesebb varrás keletkezik ott, ahol a kontúr elindul, és csökkenti a húrozást a következő mozgásban.

<!--screenshot {
"image_path": "coasting_enable.png",
"models": [{"script": "phone_holder.scad"}],
"camera_position": [0, -215, 117],
"minimum_layer": 1,
"structures": ["travels", "helpers", "shell", "infill", "starts"],
"settings": {
    "coasting_enable": true,
    "coasting_volume": 0.06,
    "z_seam_position": "backright"
},
"colours": 32
}-->

![Rétegnézetben a varrás jól látható, ha a szabadonfutás engedélyezve van, mert akkor ott mozgás van](../images/coasting_enable.png)

A gördülés engedélyezése csökkenti a falak varrásának láthatóságát. Ha általában nagy vastag varratok vannak, ennek engedélyezése csökkentheti ezt a hatást. Ez alapvetően az ellenkezője annak, amit a [külső faltörlési távolság](../shell/wall_0_wipe_dist.md) tesz, ezért érdemes először csökkenteni a törlés mértékét, mielőtt megkísérelné a szabadon mozgatást.

A kihúzás elméletileg mindig alulextrudálást eredményez. A körülményektől függ, hogy ez látható-e a tényleges nyomtatáson vagy sem. A közvetlen meghajtót használó nyomtatóknál a szabadon töltés valamivel hatékonyabb. Ha a nyomtatója közvetlen meghajtással rendelkezik, akkor érdemes alacsonyabb értékre csökkenteni a [szabadonfutó térfogatot](coasting_volume.md) , mint Bowden-csövek vagy hajlékony hajtótengelyek használatakor, mert akkor sokkal gyorsabb az áramlási sebesség reakciója. A Bowden-stílusú adagolórendszerekkel sokkal nehezebb lesz szabályozni a kifutás mértékét, hogy hatékonyan csökkentse a varrás láthatóságát.
