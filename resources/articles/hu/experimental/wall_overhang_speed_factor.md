# Túlnyúló falsebesség

Ezzel a beállítással beállítható [a túlnyúló falak](wall_overhang_angle.md) nyomtatásának sebessége. A sebesség a normál nyomtatási sebesség arányaként van beállítva, amely vagy a [külső fali sebesség](../speed/speed_wall_0.md) vagy a [belső fal sebessége](../speed/speed_wall_x.md) .

A túlnyúlás alacsonyabb sebességgel nagyon hatékonyan csökkentheti a lelógást. Ennek számos pozitív hatása van a nyomatára.

- A falaknak több ideje van az előző réteg szomszédos falaihoz tapadni. Ez segít nekik jobban függőlegesen maradni, ami csökkenti a leesést.
- Ha a ventilátor sebességét magasra állítja, a ventilátoroknak több idejük lesz az izzószál lehűtésére. Így gyorsabban megszilárdul. Ha a nyomtatási sebesség nagy volt, az anyagnak több ideje lesz leereszkedni.
- A túlnyúlásban lévő anyag továbbra is a fúvókából kilépő gyöngyhöz kapcsolódik. Lassabb nyomtatásnál a fúvóka közelebb marad a megszilárdulás során, ami azt jelenti, hogy a fúvóka húzása az anyagra hatékonyabban tartja fenn a gyöngyöt, amíg megszilárdul.

Azonban az alacsonyabb (vagy eltérő sebességű) nyomtatás túlnyúlása negatív hatással is járhat:

- A nyomtatás nyilvánvalóan tovább tart.
- A szegély, ahol a nyomtatási sebesség eltérő, kívülről nagyon jól látható lehet. Ez látható szegélyt hoz létre a nyomatban, amely nem kívánatos.
- A sebesség csökkentésekor a fúvókakamrában kialakuló nagy nyomás miatt rövid időre túlnyomás lép fel a fúvókán. Ez törésekhez vezethet, vagy ronthatja a túlnyúlás minőségét. A sebesség növelésekor némi alulextrudálás tapasztalható. Általánosságban elmondható, hogy ez a technika jobban működik a nagy túlnyúlási területeken, nem pedig a kis területeken.
