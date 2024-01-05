# Támogassa az interfész vonalirányait

A támasztófelületet általában úgy állítják be, hogy a lehető legmerőlegesebb legyen a modellre és az azt körülvevő tartótestre. Ha a felső/alsó vonalak vagy a támasztóvonalak tájolása testre szabott, célszerű a támasztó interfész vonalak tájolását is testre szabni. Ez a beállítás lehetővé teszi a támogatási interfész vonalak tájolásának testreszabását.

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

![0° és 90° szögben döntve](../images/support_interface_angles_0.png)![45°-ban és 135°-ban döntve](../images/support_interface_angles_45.png)

Ehhez a beállításhoz több szög is kitölthető, vesszővel elválasztva. A Cura ezeket a szögeket váltogatja a rétegek között.

A támasztó interfész vonalai ideális esetben merőlegesek legyenek azokra a vonalakra, amelyeken támaszkodnak, valamint a rájuk támaszkodó vonalakra. A merőleges tájolásuk csökkenti azt a távolságot, amelyet ezeknek a vonalaknak át kell hidalniuk, és így csökkenti a megereszkedést és javítja a túlnyúlások minőségét. Ez különösen fontos, ha nem teljesen sűrű támasztékkal dolgozik.
