# Maximális ventilátor sebesség

Az a sebesség, amellyel a nyomtatófejben lévő ventilátorok forognak, amikor a réteget a minimális rétegidővel nyomtatják. A minimális rétegidőnél érdemes a réteget a lehető leggyorsabban lehűteni, hogy lerövidítse a réteg lehűléséhez szükséges időt, mielőtt a nyomtató ráhelyezi a következő réteget.

![Melyik ventilátor sebességet hol használják](../images/cool_fan_speed.svg)

Ha egy réteg nyomtatása a [Normál/Maximális ventilátorsebesség küszöbértéke](cool_min_layer_time_fan_speed_max.md) és a [Minimális rétegidő](cool_min_layer_time.md) beállításai között tart, akkor a ventilátorsebesség a [normál ventilátorsebesség](cool_fan_speed_min.md) és a [maximális ventilátorsebesség](cool_fan_speed_max.md) között lesz interpolálva. A minimális rétegidő elérése után a maximális ventilátorsebesség is elérésre kerül. Így a nyomat maximálisan lehűl, hogy a lehető leggyorsabban lehűljön, mielőtt a következő réteg a tetejére kerül.
