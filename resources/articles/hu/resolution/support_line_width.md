# Támogatási vonal szélessége

Azon vonalak szélessége, amelyekkel a támaszt megrajzolják, eltérhet a nyomat többi részének vonalszélességétől.

<!--screenshot {
"image_path": "support_line_width.png",
"models": [
    {
        "script": "clamp.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [28, 57, 90],
"settings": {
    "support_enable": true,
    "support_line_width": 0.8
},
"layer": 350,
"colours": 128
}-->

![A támasztóvonalak szélesebbek, mint a többi vonal](../images/support_line_width.png)

A támasztékot általában nem kell pontosan nyomtatni, így nagyobb vonalszélességgel nyomtatható, hogy időt takarítson meg anélkül, hogy a támaszték erőssége csökkenne. A támaszték azonos sűrűségének eléréséhez azonban a vonalakat távolabb kell elhelyezni egymástól. Ez csökkenti a nyomat túlnyúló felületeinek minőségét.
