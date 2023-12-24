# Bridge Wall Flow

Ez a beállítás beállítja az áthidaló falak nyomtatásához extrudált anyag mennyiségét.

Az anyagmennyiség csökkentése hatékonyan csökkenti a rést áthidaló falak vonalszélességét. Csökkentett vonalszélességgel nagyobb a vonalak felület-tömeg aránya, ami lehetővé teszi, hogy gyorsabban lehűljenek, és ez megakadályozza, hogy annyira megereszkedjenek.

Az áramlási sebesség túlzott csökkentése azonban nagy változást okoz az áramlási sebességben, különösen, ha [lassabb nyomtatási sebességgel](bridge_wall_speed.md) párosul. A valóságban az anyag nem tudja nagyon gyorsan megváltoztatni az áramlási sebességét, ami miatt a vezetékek a tervezettnél valamivel vastagabbak lesznek az áramlási sebesség lelassulásával, és valamivel vékonyabbak a tervezettnél, ahogy az áramlási sebesség felgyorsul. Ezen hatások közül az első kompenzálható némi [kifutással](bridge_wall_coast.md) , de ez alapos hangolást igényel.
