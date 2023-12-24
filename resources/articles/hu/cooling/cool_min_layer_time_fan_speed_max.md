# Normál/maximális ventilátorsebesség küszöbértéke

Ez a beállítás határozza meg annak a rétegnek a nyomtatási idejét, amelynél az annyira rövid, hogy a ventilátor sebessége a [Maximális ventilátorsebesség](cool_fan_speed_max.md) felé kezd növekedni. Azok a rétegek, amelyek nyomtatása ennél hosszabb ideig tart, a [normál ventilátorsebességet](cool_fan_speed_min.md) használja. Azoknál a rétegeknél, amelyek nyomtatása rövidebb, a ventilátor sebessége a normál és a maximális ventilátorsebesség között interpolálódik, egészen a [minimális rétegidő](cool_min_layer_time.md) felé, ahol a ventilátor sebessége a maximális ventilátorsebesség mellett lesz.

![Melyik ventilátor sebességet hol használják](../images/cool_fan_speed.svg)

Ennek a küszöbértéknek a csökkentése (rövidebb rétegek felé) gyakorlatilag azt eredményezi, hogy a ventilátor gyakrabban forog a szokásos ventilátorsebességgel. Ennek a küszöbértéknek a növelésével a ventilátor gyakrabban fog nagyobb sebességgel forogni, még akkor is, ha a rétegek nem túl kicsik.

Jó bizonyos távolságot tartani a minimális rétegidő és a normál/maximális ventilátorsebesség küszöb között. Ha a küszöbértéket a minimális rétegidőre állítja be, a ventilátor hirtelen leáll, ha a rétegek valamivel a küszöb alá kerülnek. Ez látható sávokat okoz a nyomat felületén, mivel van egy kemény szegély, ahol a ventilátor hirtelen fellángolt. Ha ehelyett van némi eltérés a két beállítás között, a ventilátor sebességének változása fokozatosabb lesz, és a sávozás nem lesz látható a nyomtatáson.
