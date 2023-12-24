# Kifutási sebesség

A kifutás során a fúvóka nem extrudál tovább. Ez azonban nem egészen utazásként viselkedik. A fúvóka továbbra is megközelítőleg azonos sebességgel halad tovább. Ezzel a beállítással konfigurálható a pontos sebesség, amellyel a fúvóka továbbhalad.

A szabadonfutás sebességét a normál nyomtatási sebesség aránya határozza meg. Ez azt jelenti, hogy ha a [külső fal](../speed/speed_wall_0.md) és [a belső fal](../speed/speed_wall_x.md) különböző sebességű, akkor ezek is eltérő sebességgel fognak kifutni. Az alulextrudálás leküzdése érdekében a szabadon mozgatást általában a normál nyomtatási sebességnél valamivel alacsonyabb sebességgel végzik.

A szabadonfutás sebességének csökkentése csökkenti az alulextrudálási hatást, amelyet a szabadonfutás természetesen okoz a fal során, de növeli az alulextrudálási hatást, miután a fúvóka a következő szerkezet nyomtatására vált, mivel a fúvóka hosszabb ideig szivárog. A csökkentett sebesség a legjobb párosítani a csökkentett [térfogattal](coasting_volume.md) a szabadonfutáshoz, hogy a fúvóka ne maradjon túl sokáig szivárogva.

A sebesség csökkentése csökkenti a szabadonfutás hatását is, mivel a fúvóka hosszabb ideig támaszkodik a varraton. Ez jobban láthatóvá teszi a varrást.
