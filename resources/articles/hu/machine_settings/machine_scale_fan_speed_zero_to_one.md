# A ventilátor sebességét 0-1-re skálázza

A nyomtató ventilátorainak forgási sebességének szabályozására a Cura parancsokat ad a g-kódba a sebességet szabályozó paraméterrel. Általában ez a paraméter egy 0 és 255 közötti szám. Egyes nyomtatók azonban elfogadnak egy 0 és 1 közötti számot is, és akkor másképp értelmezik. Ezzel a beállítással a Cura 0 és 1 közötti számként írja be a ventilátorsebességeket 0 és 255 közötti számok helyett.

A firmware-nek háromféle viselkedése létezik a piacon lévő különféle nyomtatókban.

- A legtöbb nyomtató a ventilátorsebességeket csak 0 és 255 közötti számként fogadja el. Ezt a beállítást ilyenkor le kell tiltani, különben a ventilátor soha nem fog igazán forogni.
- Egyes nyomtatók (különösen a RepRapFirmware) elfogadnak 0 és 255 közötti számokat, de ha ez 1 vagy kisebb, akkor 0 és 1 közötti számként értelmezze. Ezt a beállítást akkor kell engedélyezni, különben előfordulhat olyan ritka eset, amikor Cura megpróbálja beállítani a ventilátor sebessége 0,4% (255-ből 1), de a nyomtató 100%-ra állítja be.
- Egyes nyomtatók csak 0 és 1 közötti számokat fogadnak el. Ezt a beállítást akkor is engedélyezni kell, különben a ventilátor mindig teljesen kikapcsolt vagy teljesen bekapcsolt állapotban lesz.
