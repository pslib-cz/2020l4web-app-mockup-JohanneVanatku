# Hra SHOOTEM
Hra SHOOTEM je inspirována množstvím starých her z 80. let a především hrou Space Invaders. Hráč ovládá několik děl na levé straně obrazovky a jeho úkolem je střílet na nepřátelé přicházející z pravé strany. Děla nemohou mířit a nepřátelé přicházejí v řadách, hráč tedy musí vybrat dělo ve správné řadě a střílet.

## Mechanika
Na začátku hry má hráč 2 děla a dvě řady nepřátel. Nepřátelé přichází z pravé strany obrazovky a postupně se blíží. Pokud překročí modrou čáru napravo, zmizí a hráč přichází o jeden život.  Hráč si šipkami může zvolit dělo a tlačítkem „S“ z něj vystřelit, střela vždy zasáhne nejbližšího nepřítele v řadě. Hráč nemůže spamovat střely, po každém výstřelu by měl následovat cooldown, než bude možné z toho samého děla znovu vystřelit (např 0.5 - 1s).
Hra má 4 levely. S každým levelem se zvýší počet řad (a i děl) a objeví se nový druh nepřátel. Na konci každého levelu je boss, který má více životů a po každém zásahu má šanci změnit svou pozici v řadách.
Hráč má 4 životy. Pokud se nepřítel dostane za modrou čáru, přichází o 1 život. Pokud se boss dostane za modrou čáru, hráč umírá, nehledě na počet životů. Na každém novém levelu se vyléčí na plný počet životů.
Hlavním cílem hry je získat si co nejvyšší skóre. To je vypočítáváno počtem zabitých nepřátel a počtem ztracených životů.

## Druhy nepřítel:
Každý level má vlastní sadu nepřátel a každá sada má normálního nepřítele (def), racera, tank a bosse.
- Normální nepřítel - pohybuje se normální rychlostí, má 1 HP
- Racer - pohybuje se dvakrát rychleji, než normální nepřítel, má 1 HP
- Tank - pohybuje se normální rychlostí, má 2 HP
- Boss - objeví se na konci levelu, žádný jiný nepřítel není přítomen při bossfightu, má 4 až 7 HP (podle levelu), po každém zásahu má náhodnou šanci na změnu řady.

## Levely:
Hra má 4 levely. První level má dvě řady nepřátel a dvě děla, druhá tři.. Poslední 4. level má 5 řad. Každý level má vlastní sadu nepřátel a vlastní barvu (červená > žlutá > tyrkysová > magenta).  Aby hráč mohl postoupit do dalšího levelu, musí zabít určitý počet nepřátel (20 > 25 > 30 > 35) a bosse daného levelu. Momentální postup se zobrazuje na panelu v pravém horním rohu.  Při každém novém levelu se hráč vrátí na plný počet životů. Po posledním levelu se mu ukáže obrazovka s jeho skóre.

## Levely - Nepřítelé:
Množství určitých druhů nepřátel je pro každý level dán v poměru 3:1:1 (normální:racer:tank). První level má tedy 12 normálních nepřátel, 4 racery a 4 tanky, druhý 15 norm., 5 racerů a 5 tanků atd. Nepřátelé by měli být náhodní. Nový nepřítel by se měl objevit vždy 1 - 2 sekundami).
Normálnímu nepříteli a tanku by překročení obrazovky mělo trvat zhruba 10 sekund, racerovi zhruba 5. Bossovi prvního levelu by to mělo zabrat téže 13 sekund, ale v dalších levelech by se jeho čas měl prodlužovat (16 > 21 > 25). Toto je ale jen odhad a rychlost nepřátel je možné po testování upravit.

## Výpočet skóre:
Za každého poraženého nepřítele hráč získává 50 bodů, za každého bosse 150 bodů. Za každý ztracený život ztrácí 100 bodů. Momentální skóre se zobrazuje na panelu v pravém horním rohu obrazovky a poté na obrazovce "You win!" a "Game over".

## Grafika a animace:
Všechny animace hrají v 10fps a jsou očíslovány v pořadí. Hra má grafiku ve velmi malám rozlišení a pouze 16 barev z inspirace ze staré limitované grafiky. Hra obsahuje i červený sprite pro dělo, když střílí a zelený pro vybrané dělo, sprite pro prázdný HP slot a font pixel operator.
### Barvy:
Barvevná paleta pochází z grafické karty EGA  
#ffffff bílá, #aaaaaa světle šedá, #555555 tmavě šedá, #000000 černá, #ff55ff růžová/světlá magenta, #aa00aa tmavá magenta, #5555ff modrá, #0000aa tmavě modrá, #55ffff tyrkysová, #00aaaa tmavě tyrkysová, #55ff55 světle zelená, #00aa00 tmavě zelená, #ffff55 žlutá, #aa5500 hnědá, #ff5555 světle červená , #aa0000 tmavě červená
### Zvuky
Hra obsahuje i několik zvuků pro zničení nepřítele, střílení, přicházejícího bosse apod.

Úvodní obrazovka:  
![Úvodní obrazovka](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/TitleScreenMenuEXA.png)

Screenshot ze hry:  
![Screenshot ze hry](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/screen.png)

Výherní obrazovka:  
![Výherní obrazovka](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/ScoreScreenEXA.png)

Game over:  
![Game over](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/game%20overEXA.png)

Začínající bossfight:  
![Začínající bossfight](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/Boss%20incoming.png)

Rozložení děl:  
![Rozložení děl](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/cannons.png)

Nepřátelé:  
![Nepřátelé](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/nep%C5%99%C3%A1tel%C3%A9.png)


Ukázky animací:  
![Boss 1](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/boss1ANIM.gif)
![Boss 2](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/boss2ANIM.gif)
![exploze](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/exploANIM.gif)
![nepřítel](https://github.com/pslib-cz/2020l4web-app-mockup-JohanneVanatku/blob/master/uk%C3%A1zky/enemyANIM.gif)
