# Belső fal(ak) Vonalszélesség

A belső falak vonalszélessége a külső faltól külön állítható. Ez a beállítás azt jelzi, hogy az egyes belső falvonalak milyen szélesek lesznek.

<!--screenshot {
"image_path": "wall_line_width_x.png",
"models": [{"script": "hive.scad"}],
"camera_position": [-31, -31, 147],
"settings": {
    "wall_line_count": 3,
    "wall_line_width_x": 0.8
},
"colours": 64
}-->

![A belső falak vonalai sokkal szélesebbek, mint a többi](../images/wall_line_width_x.png)

A belső falak vonalszélességének kicsinyítése a fúvóka mérete alatt ismert, hogy előnyös a szilárdság szempontjából. A fúvóka valamivel kevesebb anyagot extrudál, de a nyílása átfedi a szomszédos falvonalakat. Ez azt eredményezi, hogy az anyagot a korábban felhelyezett fal félretolja a megfelelő helyére. De ettől a műanyag jobban összeolvad a szomszédos falakkal. Ez lehetővé teszi, hogy a falak jobban összeolvadjanak, hogy egyesíthessék erejüket. Ez nagymértékben javítja a falak szilárdságát.

A belső fal vonalszélességének növelése csökkentheti a nyomtatási időt. Hasonló erősségű alkatrészekhez kevesebb belső falra lesz szükség. A szilárdság továbbra is némileg csökken, mivel a szomszédos falak nem olvadnak össze annyira.


<comment></comment>Vékony részeken a vonal szélessége automatikusan beállítódik, hogy illeszkedjen az ott található alkatrész helyi szélességéhez. Nem szükséges biztosítani, hogy az alkatrész szélessége a vonal szélességének többszöröse legyen. A [Wall Transitioning Threshold Angle] (../shell/wall_transition_angle.md) határozza meg, hogy az éles sarkokban hol kerül automatikusan beállításra a vonalszélesség. A [Minimum Wall Line Width] (../shell/min_wall_line_width.md) határozza meg, hogy milyen messzire állíthatók be az egyes irányokba.<comment></comment>

<!--if cura_version<5.0:
Making lines fit
----
When printing thin parts, adjusting the wall line width settings is an important tool to get accurate and strong parts. Cura will only ever draw complete contours, so if a contour doesn't fit a gap will fall into the walls, which greatly compromises the strength and accuracy of the part.

Cura will attempt to fill such gaps between walls if [Fill Gaps Between Walls](../shell/fill_perimeter_gaps.md) is enabled, but that technique is less than ideal for arbitrary shapes and often takes a lot of printing time. When two walls overlap, the [Compensate Wall Overlaps](../shell/travel_compensate_overlapping_walls_enabled.md) feature will reduce the wall line width to make sure that the part is dimensionally accurate, but this incurs flow changes which reduce the quality and strength of the print as well.

For an ideal fit you want the part to be an exact multiple of the wall line width so that the walls fit precisely within the part. If you know how wide your part is, this can easily be done by adjusting the width of the walls. First you see how many contours you want to fit such that the lines still have a reasonable width. Then you can see how much you need to adjust the wall line width to make the lines fit properly. Keep in mind that you can adjust the [Outer Wall Line Width](wall_line_width_0.md) and [Inner Wall Line Width](wall_line_width_x.md) separately. Count carefully how many times each type of wall will be drawn to predict the effect of changing the wall line width.

Fitting wall lines is an important skill for 3D printing that distinguishes expert 3D printer operators from the rest. Some practice is required.-->
