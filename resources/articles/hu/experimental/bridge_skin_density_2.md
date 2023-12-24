# Híd második bőrsűrűsége

Ez a beállítás szabályozza a bőr sűrűségét a híd feletti második rétegben. 100%-os sűrűségnél a vonalak közvetlenül egymás mellett helyezkednek el. Kisebb sűrűségnél a vonalak távolabb helyezkednek el egymástól.

Ha a bőrvonalak közvetlenül egymás mellett helyezkednek el, akkor egymáshoz tapadnak. Ez segít a modell vízállóvá tételében, és simábban fog kinézni a nyomat alsó oldalán. Azt is lehetővé teszi, hogy a következő sorok kissé az előző sorokra támaszkodjanak, ami segít megelőzni a megereszkedést.

Az anyag azonban nem tud lehűlni. A bőrvonalak közötti távolsággal a levegő képes lesz a gyöngyök körül áramolni, ami jelentősen javítja a gyöngyök lehűlésének és megszilárdulásának sebességét. Természetesen ez csak akkor érvényes, ha a ventilátor be van kapcsolva, így a magas hőmérsékletű anyagok esetében ez a stratégia nem működik. A megereszkedési hatás a második rétegben is csökken, mert az elsőre támaszkodhat, így az egyéb tényezők, mint például a simaság, inkább ennél a rétegnél számítanak. Vegye figyelembe azt is, hogy egy bizonyos ponton valószínűleg azt akarja majd, hogy az alsó oldal teljesen bezáruljon, hogy vízzáróvá váljon, vagy sima legyen.

Hogy ezek közül melyik hatás erősebb, az az anyag viszkozitásától, a megszilárdulás sebességétől és a ventilátor sebességétől függ. Némi hangolás mindig szükséges.

**Ha a [Bridge Second Skin Flow](bridge_skin_material_flow_2.md) kisebb, mint 100%, akkor is lesz némi távolság a vonalak között, még akkor is, ha a sűrűség 100%, mert akkor a vonalak vékonyabbak lesznek.**
