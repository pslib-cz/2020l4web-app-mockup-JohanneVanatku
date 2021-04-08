# Hra SHOOTEM
Hra SHOOTEM je inspirována množstvím starých her z 80. let a především hrou Space Invaders. Hráč ovládá několik děl na levé straně obrazovky a jeho úkolem je střílet na nepřátelé přicházející z pravé strany. Děla nemohou mířit a nepřátelé přicházejí v řadách, hráč tedy musí vybrat dělo ve správné řadě a střílet.

## Mechanika
Na začátku hry má hráč 2 děla a dvě řady nepřátel. Nepřátelé přichází z pravé strany obrazovky a postupně se blíží. Pokud překročí modrou čáru napravo, zmizí a hráč přichází o jeden život.  Hráč si šipkami může zvolit dělo a tlačítkem „S“ z něj vystřelit, střela vždy zasáhne nejbližšího nepřítele v řadě.
Hra má 4 levely. S každým levelem se zvýší počet řad (a i děl) a objeví se nový druh nepřátel. Na konci každého levelu je boss, který má více životů a po každém zásahu má šanci změnit svou pozici v řadách.
Hráč má 4 životy. Pokud se nepřítel dostane za modrou čáru, přichází o 1 život. Pokud se boss dostane za modrou čáru, hráč umírá, nehledě na počet životů. Na každém novém levelu se vyléčí na plný počet životů.
Hlavním cílem hry je získat si co nejvyšší skóre. To je vypočítáváno počtem zabitých nepřátel a počtem ztracených životů.

## Druhy nepřítel:
Každý level má vlastní sadu nepřátel a každá sada má normálního nepřítele (def), racera, tank a bosse.
Normální nepřítel - pohybuje se normální rychlostí, má 1 HP
Racer - pohybuje se rychleji, než normální nepřítel, má 1 HP
Tank - pohybuje se normální rychlostí, má 2 HP
Boss - objeví se na konci levelu, žádný jiný nepřítel není přítomen při bossfightu, má 4 až 8 HP (podle levelu), po každém zásahu má náhodnou šanci na změnu řady.

## Levely:
Hra má 4 levely. První level má dvě řady nepřátel a dvě děla, druhá tři.. Poslední 4. level má 5 řad. Každý level má vlastní sadu nepřátel a vlastní barvu (červená > žlutá > tyrkysová > magenta).  Aby hráč mohl postoupit do dalšího levelu, musí zabít určitý počet nepřátel (20 > 25 > 30 > 35) a bosse daného levelu. Momentální postup se zobrazuje na panelu v pravém horním rohu.  Při každém novém levelu se hráč vrátí na plný počet životů. Po posledním levelu se mu ukáže obrazovka s jeho skóre.

## Výpočet skóre:
Za každého poraženého nepřítele hráč získává 50 bodů, za každého bosse 150 bodů. Za každý ztracený život ztrácí 100 bodů. Momentální skóre se zobrazuje na panelu v pravém horním rohu obrazovky a poté na obrazovce "You win!" a "Game over".

## Grafika a animace:
Všechny animace hrají v 10fps a jsou očíslovány v pořadí. Hra má grafiku ve velmi malám rozlišení a pouze 16 barev z inspirace ze staré limitované grafiky. Hra obsahuje i sprite pro dělo, když střílí, sprite pro prázdný HP slot a font 8bit operator.
