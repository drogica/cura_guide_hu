# Törölje le a fúvókát a rétegek között

Ez a beállítás lehetővé teszi egy olyan eljárást, amely minden réteg végén végrehajtódik, és letöröl minden anyagot a fúvóka hegyéről. Ha beépített törlőkefével rendelkező nyomtatója van, ennek a beállításnak az engedélyezése azt eredményezi, hogy a Cura utasítja a nyomtatót, hogy időnként törölje le az adott keféről a fúvókát.

![A törlési eljárás mozdulatainak megjelenítése](../images/clean_between_layers.svg)

Ez a törlési eljárás több lépésből áll:

1. Ha [a visszahúzás engedélyezve van](wipe_retraction_enable.md) , az anyag visszahúzódik.
2. Ha [a Z-hop engedélyezve van](wipe_hop_enable.md) , a fúvóka felfelé, vagy az építőlemez lefelé mozog.
3. A fúvóka túl van [a kefe pozícióján](wipe_brush_pos_x.md) .
4. A fúvókát [többször](wipe_repeat_count.md) le kell törölni a keféről.
5. A fúvóka visszakerül eredeti helyzetébe.
6. A Z ugrás véget ért, ha engedélyezve volt. Az anyag visszahúzódik.
7. A nyomtatás egy [bizonyos ideig](wipe_pause.md) szünetel.

Ennek az eljárásnak az a célja, hogy a fúvókát rendszeresen megtisztítsa a törmeléktől. Egyes anyagok hajlamosak a nagy felületi feszültség miatt kapillárisan felkúszni a fúvókához. Ez bekúszhat a nyomtatófejbe és ott összegyűlhet, ami széttörheti a nyomtatófejet. Más szálakat vagy más tölteléket tartalmazó anyagok nyomtatás közben a tölteléket a fúvókára permetezhetik. Ez letörli az anyagot.

A törlési eljárás azonban most nem nagyon konfigurálható. Mindig X irányban törli, megtartva a nyomtatás utolsó pozíciójának Y pozícióját. Ez azt jelenti, hogy a sarokban lévő ecsettel rendelkező nyomtató nem fog jól működni ezzel a funkcióval. Szüksége lesz egy kefére az építési térfogat teljes oldalán.
