# A Support Brim engedélyezése

Amikor a tartóperem aktiválva van, egy további perem rajzolódik ki az első réteg támasztóterületén belül.

<!--screenshot {
"image_path": "support_brim_4mm.png",
"models": [{"script": "gazebo2.scad"}],
"camera_position": [-74, 38, -137],
"settings": {
    "support_enable": true,
    "support_use_towers": false,
    "support_brim_enable": true,
    "support_brim_width": 4
},
"colours": 64
}-->

![A tartóperem](../images/support_brim_4mm.png)

A támasztóperem a közönséges *karimával* ellentétben befelé húzódik. Ha az [Építőlemez tapadási típusa](../platform_adhesion/adhesion_type.md) peremre van állítva, egy másik perem is rajzolódik a támasz *köré* .

Ennek a peremnek az a célja, hogy a tartónak nagyobb felületet biztosítson, ahol hozzá tud tapadni az építőlemezhez. Ez elérhető az [Initial Layer Support Line Distance](support_initial_layer_line_distance.md) beállításával is, de ezzel a funkcióval a tapadás a támasztófelület széle körül összpontosul, ahol hatékonyabban lehet megakadályozni a vetemedést.

A tartóperem kis mértékben növeli a nyomtatási időt és az anyagköltséget is, de mivel csak az első rétegen van, ez nagyon minimális. Jelentősen megerősíti a támasztékot, így a cikkcakk tartómintánál nehezebb lesz a letörés.
