# A Draft Shield engedélyezése

Ha ez a beállítás engedélyezve van, a nyomtató egy héjat épít a nyomat köré, amely megvédi a nyomatot a környezettől érkező légáramoktól.

<!--screenshot {
"image_path": "draft_shield_enabled.png",
"models": [{"script": "headphone_hook.scad"}],
"camera_position": [-56, 139, 305],
"settings": {
    "draft_shield_enabled": true
},
"colours": 32
}-->

![A modell köré huzatvédő van nyomtatva](../images/draft_shield_enabled.png)

Egyes nyomtatók és nyomtatási anyagok nagyon érzékenyek a környezetre, amelyben nyomtatnak. Az építőlemez különböző helyeire történő nyomtatás eltérő eredményekhez vezethet, mivel érzékenyebbek a kívülről érkező légáramlatokra. Ha a nyomat egy éjszakán át futni hagyja, és a helyiség lehűl, ez jelentősen befolyásolhatja a nyomatot. A huzatvédő pajzs ezt a hatást hivatott csökkenteni azáltal, hogy kis, elszigetelt térfogatot hoz létre a nyomat körül. Ez ideiglenes "fűtött kamraként" szolgál, hogy melegen tartsa a nyomatot, és megvédje a kívülről érkező hideg léghuzattól.

A pajzsot menet közben nyomtatják, ahogy a modellt nyomtatják. Ha több extruder is részt vesz a nyomtatásban, a huzatvédőt a réteget elindító extruder segítségével nyomtatja ki. Ez rétegről rétegre váltakozik.

A huzatpajzsnak számos jelentős hatása van a nyomtatásra:

- A nyomat hőmérsékletét állandóbban tartja. Ez a huzatvédő pajzs tervezett hatása. Ennek eredményeként csökkenteni kell a helyiség hőmérséklet-eltolódása miatti sávosodást.
- Általában a huzatvédő pajzs belsejében a hőmérséklet magasabb, mint ha nincs huzatvédő pajzs. Ennek az az oka, hogy a hő nehezebben szökik ki, és nem tud felszállni konvektív áram a forró levegővel a nyomatból. Ez a nyomtatás minden aspektusára hatással van. Különösen nagyobb lesz a húrozás és a megereszkedés.
- A nyomtatófej ventilátorai kevésbé hatékonyak. A pajzs az ottani légáramlást is megzavarja. A nyomtatófejen lévő ventilátorok hatékonyságának növelése érdekében a huzatpajzs [távolsága](draft_shield_dist.md) növelhető.
- A huzatpajzs dupla [szivárgáspajzsként](../dual/ooze_shield_enabled.md) is funkcionálhat. Ha egy olyan tárgy felé halad, amelyet huzatvédő pajzs véd, a fúvókán maradt szivárgás letörlődik a pajzsról.
- A huzatpajzs [Prime Towerként](../dual/prime_tower_enable.md) is funkcionálhat. Mivel a tárgy előtt van kinyomtatva, a huzatpajzs nyomtatása egy módja annak, hogy az anyagot kitisztítsák és megfelelően folyjon. Ez azonban csak 2 extruder esetén hatásos, mivel nem minden extruder ürül ki, ha kettőnél több van.
