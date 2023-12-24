# Vonalvastagság

Ez azon vonalak vízszintes szélessége, amelyeket a nyomtató le fog helyezni. Általában a fúvókanyílás átmérője határozza meg, hogy milyen szélesek lesznek a vonalak, de több-kevesebb anyag extrudálásával a nyomtató egy kicsit változhat a vonalak szélességét illetően.

<!--screenshot {
"image_path": "line_width_small.png",
"models": [{"script": "holes_cutout.scad"}],
"camera_position": [17, 39, 61],
"settings": {"line_width": 0.2},
"colours": 64
}-->

<!--screenshot {
"image_path": "line_width_large.png",
"models": [{"script": "holes_cutout.scad"}],
"camera_position": [17, 39, 61],
"settings": {"line_width": 0.6},
"colours": 32
}-->

![Nagyon vékony vonalak](../images/line_width_small.png)![Nagyon széles vonalak](../images/line_width_large.png)

A vonalszélesség csökkentése lehetővé teszi a nyomtató számára, hogy több részletet nyomtasson ki. Különösen lehetővé teszi a nyomtató számára, hogy vékony részeket nyomtasson. A vonalszélesség az egyik legbefolyásosabb beállítás a nyomtatásban. Íme néhány hatás:

- A vékonyabb vonalak nyomtatása lehetővé teszi vékonyabb darabok nyomtatását, mivel a legvékonyabb részeken akár egy vonal is elfér.
- Ha a vonalszélességet a nyomat vastagságának többszörösére állítja, akkor a tárgy erősebb lesz, és az anyag jobban folyhat.
- A kisebb vonalszélesség simábbá teszi a felső felületet.
- A fúvóka méreténél valamivel kisebb vonalak nyomtatása általában javítja a szilárdságot. Lehetővé teszi, hogy a fúvóka összeolvasztja a szomszédos vonalakat, amikor egy második lépést hajt végre kissé az előző vonalon.
- A túl széles vonalak alulextrudáláshoz vezetnek. A nyomtató megpróbál több anyagot extrudálni, ami elegendő ahhoz, hogy kitöltse a vonal kívánt szélességét. Ez az anyag megkísérli az áramlást olyan irányba, ahol csak tud. Egy ponton azonban az ellennyomás túl nagy lesz, így az anyag már nem folyik egészen a nagyon széles vonalak oldaláig. Ez aztán hézagokat hagy a sorok között.
- A túl kicsi nyomtatási vonalak szintén alulextrudáláshoz vezetnek. Ha az anyag nem folyik át elég gyorsan a fúvókán, az anyag felületi feszültsége miatt kis cseppekké koagulálódik, ami egyenetlenné teszi az extrudálást, és hézagokat hagy a cseppek között.
- Vékonyabb vonalak nyomtatása jelentősen megnöveli a nyomtatási időt.

Nem tanácsos a vonalszélességet a fúvóka méretének 60%-a alá vagy 150%-a fölé csökkenteni. Előfordulhat, hogy mindkettő nem extrudál elegendő anyagot.


<comment></comment>Vékony részeken a vonal szélessége automatikusan beállítódik, hogy illeszkedjen az ott található alkatrész helyi szélességéhez. Nem szükséges biztosítani, hogy az alkatrész szélessége a vonal szélességének többszöröse legyen. A [Wall Transitioning Threshold Angle] (../shell/wall_transition_angle.md) határozza meg, hogy az éles sarkokban hol kerül automatikusan beállításra a vonalszélesség. A [Minimum Wall Line Width] (../shell/min_wall_line_width.md) határozza meg, hogy milyen messzire állíthatók be az egyes irányokba.<comment></comment>

<!--if cura_version<5.0:
Adjusting line widths to fit enough walls
----
When printing mechanical objects that need to be thin but strong, you'll regularly run into the problem that your piece is not a clean even multiple of the line width. If it's not an even multiple, Cura will normally reduce the flow of some of the lines due to the [Compensate Wall Overlaps](../shell/travel_compensate_overlapping_walls_enabled.md) setting. This changes the flow rate through the nozzle which is detrimental to visual quality. If it is a clean multiple of the line width but not an even number, one of the walls will get reduced to 0.

Producing clean contours with even lines can make the print stronger and look better. A hallmark skill of any expert Cura user is to be able to tweak the line width such that the desired number of contours fill the print.

![Default line width, where the contours don't fit and some lines are thicker than others](../images/line_width_fit_bad.png)
![Reducing the line width makes it fit evenly](../images/line_width_fit_good_small.png)
![Increasing the line width also works](../images/line_width_fit_good_large.png)
-->

## Az áramlás állandó tartása

Az áramlás nagy ingadozása néha problémát jelent az FDM nyomtatók számára. A fúvókakamra bizonyos anyagokat nyomás alatt tart, ami késlelteti a fúvókán való tényleges áramlási sebességet. Eltart egy ideig, amíg az áramlási sebesség nő vagy csökken. Az izzószál adagolására Bowden rendszerrel rendelkező nyomtatóknál a Bowden cső is ruganyos, ami sokkal rontja a hatást. Ennek eredményeként nagyobb áramlási sebességre való áttéréskor alulextrudálást, kisebb áramlási sebességre való váltáskor pedig túlextrudálást kap. Ezért célszerű az áramlási sebességet a lehető legállandóbb szinten tartani.

A vonal szélessége nagymértékben befolyásolja az áramlási sebességet. A vonalak szélességét célszerű egymáshoz közel tartani és a fúvóka méretéhez közelíteni. Ha jelentősen módosítja a vonalszélességet, akkor érdemes lehet a nyomtatási sebességet is módosítani, hogy az áramlási sebesség állandóbb legyen. Ez javítja a nyomat méretpontosságát.
