# Az adaptív rétegek maximális variációja

Ezzel a beállítással korlátozhatja azt a tartományt, amelyből az Adaptive Layers választhat rétegvastagságot. A rétegmagasság nem térhet el ennél az eltérésnél nagyobb mértékben a normál [rétegmagasságtól](../resolution/layer_height.md) .

Például 0,15 mm-es normál rétegmagasság és 0,1 mm-es eltérés esetén az Adaptive Layers 0,05 mm és 0,25 mm közötti vastagságú rétegeket készíthet.

Ez a beállítás korlátozza az Adaptive Layers funkció teljesítményét. Ha a rétegvastagság tartománya túl szűk, akkor a rétegvastagság mindig nagyon közel lesz az eredeti rétegvastagsághoz, ahogyan azt a Rétegmagasság beállítás beállította. Az adaptív rétegek nem sokat segítenek időt takarítani vagy javítani a minőségen.

Ha azonban a tartomány nagyon széles, a rétegek nagyon vastagok vagy nagyon vékonyak lehetnek. A nagyon vastag rétegek sok kiáramlást igényelnek a fúvókából, ami nem mindig lehetséges a fúvóka korlátozott mérete és a nyomtatófej fűtőpályájának olvasztási kapacitása miatt. Nagyon vékony rétegek szintén nem mindig lehetségesek az anyag viszkozitása vagy a Z tengely pontatlansága miatt. Ezért célszerű korlátozni azt a tartományt, amelyre az Adaptive Layers beállíthatja a rétegvastagságot. Ellenkező esetben a nyomtató nehezen éri el a kívánt rétegvastagságot.

A rétegvastagság soha nem mehet 0,001 mm alá, még akkor sem, ha a tartomány ezt megengedné.
