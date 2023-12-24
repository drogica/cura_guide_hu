# Hídfal borítás

A falvonalakkal történő áthidaláskor, közvetlenül a híd nyomtatása előtt, az anyagadagolás egy pillanatra szünetel. Ezalatt az idő alatt a fúvókakamrában maradt anyag kifolyik, hogy csökkentse a fúvókakamrában lévő nyomást. Ezt a technikát [kifutásnak](coasting_enable.md) nevezik. Ezzel a beállítással szabályozható a szabadonfutás mértéke. Lényegében ez szabályozza, hogy a híd előtt mennyivel áll le az anyag áramlása.

A híd elkészülte után a nem extrudált anyagot úgyis eltávolítják. Az anyagextrudálás teljes mennyisége változatlan marad. Ez visszaállítja a nyomást a fúvókára, ami megakadályozza az alulextrudálást.

<!--screenshot {
"image_path": "bridge_skin_density_100.png",
"models": [{"script": "bridge.scad"}],
"layer": 80,
"settings": {
    "bridge_settings_enabled": true,
    "bridge_skin_density": 100,
    "bridge_skin_material_flow": 100,
    "bridge_wall_material_flow": 100
},
"camera_position": [0, 18, 79],
"colours": 64
}-->

![Nincs extrudálás a híd egyik oldalán, és extra extrudálás a másik oldalon](../images/bridge_skin_density_100.png)

Ennek a beállításnak az egysége nem intuitív. A híd előtti távolság, amelynél az anyag leáll, számos tényezőtől függ:

- A fal hossza eddig, egészen a hídig. Minél hosszabb a fal, annál jobban meg tud szabadulni.
- Az áramlási sebesség a fúvókán a normál fal alatt, amely függ a falak [sebességétől](../speed/speed_wall.md) , [vonalszélességétől](../resolution/wall_line_width.md) , [áramlási sebességétől](../material/wall_material_flow.md) és [rétegmagasságától](../resolution/layer_height.md) . Minél nagyobb az áramlási sebesség normál falakban, annál hosszabb a kifutási távolság.
- Az áthidalt fal során a fúvókán való kiáramlás sebessége, amely a falak [sebességétől](bridge_wall_speed.md) és [áramlási sebességétől](bridge_wall_material_flow.md) függ. Minél nagyobb az áramlási sebesség az áthidalt falakban, annál *rövidebb* a kifutási távolság.

Ez a beállítás a végső hossz szorzótényezője.

Ennek a kifutásnak az a célja, hogy csökkentse a nyomást a fúvókakamrában. Erre azért van szükség, mert a fúvókakamrában maradó nyomás miatt az anyag jelentős távolságra kifröccsen, mielőtt megszilárdul, amint az ellennyomás megszűnik. Ez az anyag spriccelődése megereszkedéshez vezet. Lényegében a túlnyúló vonalakat a fúvókán belül maradó anyag többi része lenyomja. Ha a fúvókakamrán belüli nyomást csökkentjük, ez az erő is csökken, és kisebb lesz a megereszkedés.

A kifutás mértékének növelése csökkenti a nyomást a fúvókakamrában, mire a hídra nyomtatni kell, ami csökkenti a megereszkedés mértékét. A nyomtatás pontosabb lesz. Azonban, ha túlzottan megnöveljük a kihúzás mértékét, az alulextrudálási időszakot eredményez közvetlenül a híd nyomtatása előtt. Mivel ez az alulextrudálás a nyomat falaiban található, nagyon jól látható lesz a nyomat oldalán.
