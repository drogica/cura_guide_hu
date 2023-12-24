# Távolítsa el a tutaj belső sarkait

Ha ez a beállítás engedélyezve van, a tutaj minden belső sarka teljesen eltávolítódik, így a tutaj [domborúvá](https://en.wikipedia.org/wiki/Convex_set) válik. A tutajnak csak külső sarkai lesznek.

<!--screenshot {
"image_path": "raft_remove_inside_corners.png",
"models": [{"script": "microwave_hook.scad"}],
"camera_position": [59, 59, 200],
"settings": {
	"adhesion_type": "raft",
	"raft_remove_inside_corners": true
},
"colours": 64
}-->

![A tutaj már nem követi a modell alakját](../images/raft_remove_inside_corners.png)

Ez gyakorlatilag egyenértékű a nagyon magas [simítással](../platform_adhesion/raft_smoothing.md) . A tutaj belső sarkainak eltávolítása számos hatással jár:

- Már nem lehetséges, hogy a tutaj egy kis része messze túlnyúljon a tutaj többi részén. A tutaj kis részei nagyobb valószínűséggel leválnak az építőlemezről, különösen erősen vetemedő anyagok esetén. A belső sarkok eltávolítása csökkenti ezt a hatást, így a nyomtatás megbízhatóbbá válik.
- A tutaj nagyobb, növelve a teljes tapadási erőt az építőlemezhez.
- A tutaj nyomtatása tovább tart, és több anyagot használ fel.
