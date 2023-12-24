# Fuzzy Skin

Elmosódott bőrrel történő nyomtatáskor a nyomat oldalain a felületet szándékosan érdesítik. Ez egyfajta textúrát ad a nyomatnak.

<!--screenshot {
"image_path": "magic_fuzzy_skin_enabled.png",
"models": [{"script": "hexasphericon.scad"}],
"camera_position": [-61, 112, 136],
"settings": {
    "magic_fuzzy_skin_enabled": true
},
"colours": 32
}-->

![A falak ingatagnak tűnnek Cura rétegnézetében](../images/magic_fuzzy_skin_enabled.png)![A nyomtatási eredmény durva textúrájú](../images/magic_fuzzy_skin_photo.jpg)

Ez a mód véletlenszerű remegést ad a külső falhoz. A nyomtatófej véletlenszerűen rezeg, miközben a legkülső falra nyomtat. Emiatt a felület érdes tapintású. A felület csak a nyomat oldalain válik homályossá. A tetejére nincs homályosság.

A homályosság minden méretpontosságot kidob az ablakon. A nyomat minden bizonnyal nagyobb lesz, mint az eredeti modell. A homályos bőr a nyomtatást is tovább tart, mivel a nyomtatófej nagy gyorsulásnak van kitéve a külső fal nyomtatása közben.
