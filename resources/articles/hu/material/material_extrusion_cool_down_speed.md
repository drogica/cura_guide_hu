# Extrúziós lehűlési sebesség módosító

Ha [az Auto Temperature](../experimental/material_flow_dependent_temperature.md) engedélyezve van, a nyomtatási hőmérséklet a kinyomott anyag mennyiségétől függően változik.

Amikor az anyag felmelegszik a fúvókakamrában, ez elvonja a hőt a fúvókáról. Az anyag gyorsabban extrudálva több hőt von el a fúvókától. Ha a hőmérsékletszonda nincs pontosan a fúvóka csúcsán, akkor a fúvóka hőmérséklete valamivel alacsonyabb lesz az anyag extrudálása közben, mint üresjáratban, még jó PID-szabályozó mellett is.

Ez a beállítás azt írja le, hogy mennyi hő veszít a fúvókában nyomtatás közben. Az extrudálás során elvesztett többlet hőt a kívánt nyomtatási hőmérséklet g-kód szerinti növelésével kompenzáljuk. A beállítás értéke a fúvóka kialakításától, a nyomtatott anyag hőkapacitásától és az extrudálási sebességtől függ.
