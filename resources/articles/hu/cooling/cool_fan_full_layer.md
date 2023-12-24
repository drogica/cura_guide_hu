# Normál ventilátorsebesség rétegnél

A ventilátor sebessége a [kezdeti ventilátorsebesség](cool_fan_speed_0.md) értékétől indul a nyomtatás elején. A nyomtatás első néhány rétegében, amint ezt ez a beállítás határozza meg, a ventilátor sebessége fokozatosan a [normál ventilátorsebességre](cool_fan_speed_min.md) növekszik.

![Melyik ventilátor sebességet hol használják](../images/cool_fan_speed.svg)

Általában a kezdeti ventilátorsebesség jelentősen csökken, mivel a kezdeti rétegnek forrónak kell maradnia a nyomtatás során. Ha a kezdeti réteg lehűl, az anyag elkezd [vetemedni](../troubleshooting/warping.md) . Ez lehúzza az első réteget az építőlemezről, ami meghiúsítja a nyomtatást. Ha azonban a második réteg túl gyorsan hűl le, akkor is zsugorodni fog, és a nyírósúrlódás miatt felfelé húzza az első réteget, ezzel is megvetemítve a nyomatot. Ennek a beállításnak az a célja, hogy lehetővé tegye több réteg nyomtatását alacsonyabb ventilátorsebesség mellett. Ily módon a vetemedés megakadályozható mindaddig, amíg a nyomat nem lesz elég merev ahhoz, hogy ellenálljon a vetemedésnek.

- Ennek a beállításnak a növelése javíthatja [az ágy tapadását](../troubleshooting/bed_adhesion_problems.md) .
- Ha az építőlemez magas hőmérsékletre van felmelegítve, előfordulhat, hogy csökkentenie kell ezt a beállítást [az elefántláb](../troubleshooting/elephants_foot.md) vagy a szivárgás elkerülése érdekében.
