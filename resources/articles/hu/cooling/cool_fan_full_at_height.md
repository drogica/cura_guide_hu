# Normál ventilátorsebesség magasságban

A ventilátor sebessége a nyomtatás elején a [Kezdeti ventilátorsebesség](cool_fan_speed_0.md) beállítás értékétől indul. A nyomtatás első néhány rétegében, amíg el nem éri az ennél a beállításnál megadott magasságot, a ventilátor sebessége fokozatosan a [normál ventilátorsebességre](cool_fan_speed_min.md) növekszik.

![Melyik ventilátor sebességet hol használják](../images/cool_fan_speed.svg)

Normál esetben a ventilátor kezdeti sebessége jelentősen csökken, mivel a kezdeti rétegnek forrónak kell maradnia a nyomtatás során. Ha a kezdeti réteg lehűl, az anyag elkezd [vetemedni](../troubleshooting/warping.md) . Ez lehúzza az első réteget az építőlemezről, ami meghiúsítja a nyomtatást. Ha azonban a második réteg túl gyorsan hűl le, akkor is zsugorodni fog, és a nyírósúrlódás miatt felfelé húzza az első réteget, ezzel is megvetemítve a nyomatot. Ennek a beállításnak az a célja, hogy lehetővé tegye több réteg nyomtatását alacsonyabb ventilátorsebesség mellett. Ily módon a vetemedés megakadályozható mindaddig, amíg a nyomat nem lesz elég merev ahhoz, hogy ellenálljon a vetemedésnek.

A ventilátor sebességének egyszerű csökkentése az első néhány réteg alatt éles változást idézne elő a ventilátor sebességében, ami látható lenne a végső nyomat felületi minőségén. Ez sávozást hoz létre. Ehelyett a ventilátor sebessége fokozatosan a normál ventilátorsebesség felé változik.

- Ennek a beállításnak a növelése javíthatja [az ágy tapadását](../troubleshooting/bed_adhesion_problems.md) .
- Ha az építőlemez magas hőmérsékletre van felmelegítve, előfordulhat, hogy csökkentenie kell ezt a beállítást [az elefántláb](../troubleshooting/elephants_foot.md) vagy a szivárgás elkerülése érdekében.
