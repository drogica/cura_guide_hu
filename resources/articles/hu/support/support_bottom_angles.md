# Támogassa a padlóvonal irányait

A támasztópadlót általában úgy kell elhelyezni, hogy a lehető legnagyobb mértékben merőleges legyen a felette lévő támasztékra és az alatta lévő modellre. Ha a felső felületvonalak vagy a támasztóvonalak tájolását testre szabták, célszerű a támasztópadló vonalak tájolását is személyre szabni. Ezzel a beállítással testreszabhatja a támasztó padlóvonalak tájolását.

<!--screenshot {
"image_path": "support_interface_angles_0.png",
"models": [
    {
        "script": "plug.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [0, 36, 92],
"settings": {
    "support_enable": true,
    "support_interface_enable": true,
    "support_interface_pattern": "lines",
    "support_interface_angles": [0, 90]
},
"layer": 118,
"colours": 128
}-->

<!--screenshot {
"image_path": "support_interface_angles_45.png",
"models": [
    {
        "script": "plug.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [0, 36, 92],
"settings": {
    "support_enable": true,
    "support_interface_enable": true,
    "support_interface_pattern": "lines",
    "support_interface_angles": [45, 135]
},
"layer": 118,
"colours": 128
}-->

![Mind a tető, mind a padló 0°-os és 90°-os szöget zár be](../images/support_interface_angles_0.png)![Mind a tető, mind a padló 45°-os és 135°-os szöget zár be](../images/support_interface_angles_45.png)

Ehhez a beállításhoz több szög is kitölthető, vesszővel elválasztva. A Cura ezeket a szögeket váltogatja a rétegek között.

A támasztó padlóvonalak ideális esetben merőlegesek legyenek a modellvonalakra, amelyeken támaszkodnak, valamint a rajtuk nyugvó támasztóvonalakra. A merőleges tájolás csökkenti azt a távolságot, amelyet ezeknek a vonalaknak át kell hidalniuk, és így csökkenti a megereszkedést és javítja a támasz stabilitását.
