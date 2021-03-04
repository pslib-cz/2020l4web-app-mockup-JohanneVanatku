# hra SHOOTEM
- její inspirací je hra Space Invaders
- na levé straně obrazovky se nachází zeď a hráčova děla společně s modrou čarou před děly, zprava přichází nepřátelské lodě
-	děla nemohou mířit a lodě se drží jedné linky, hráč může střílet pouze z jednoho děla najednou, musí tedy měnit výběr děla
-	hráč začíná se dvěmi děly a dvěmi řadami nepřátel. Po zabití určitého množství nepřátel se dostává do dalšího levelu a získává další dělo a řadu. Maximální počet je 5 řad
-	každý level je zakončen bossem, ten má více životů a po každé střele může změnit svou pozici v řadách.
-	cílem je dokončit všechny levely s co nejvyšším skóre. To je vypočítané podle počtu zabitých nepřátel a počtu nepřátel, kteří se dostali za čáru
-	hráč má 4 životy. Pokuď se nepřátelská loď dostane za modrou čáru, ztrácí 1 život. Životy se resetují po začátku každého nového levelu

### Možné další vlastnosti:
-	každý level má své vlastní nepřátelé (rozdělené podle barev – červená, žlutá, tyrkysová, magenta)
-	nepřátelé mohou mít různé varianty, například někteří by mohli být rychlejší (racers) a někteří by měli více životů (tanks)

## Základní hra:
- má 4 levely
- hráč začíná se 2 děly a 2 řadami nepřátel
- po každém levelu získává další dělo a řadu, maximum je tedy 5 řad (1. level jsou dvě řady, 2. level jsou tři řady... 4. level je pět řad)
- hráč má 4 životy; ztrácí 1 život, pokud se nepřítel dostane za modrou čáru (což také automaticky nepřítele zabije); na začátku každého levelu se životy resetují
- pokud se boss dostane za modrou čáru, hráč prohrává, i když má plný počet životů
- nepřátelé mají 1 život
- boss má 4 životy
- po každém zásahu má boss možnost náhodně změnit svou pozici v řadách (tedy pouze vetikální pozici, jeho horizontální pozice/postup zůstává stejná)
- hraje se na skóre

## Rozšířená hra:
- existují další dva typy nepřátel: racers a tanks
- racers se pohybují dvakrát rychleji, než normální nepřítel a mají 1 HP
- tanks mají 2 HP a pohybují se stejnou rychlostí
- každý level má vlastní nepřátelé (vlastnosti zůstávají stejné, mění se pouze vzhled, to platí i pro bossy)

## Další vysvětlení mechanik:
-	může být vybráno pouze jedno dělo najednou, výběr funguje přes šipky na klávesnici, nebo kliknutím na dané dělo
-	střela se k nepříteli dostane okamžitě, není schoná nepřátelé prostřelit. Střílí se pomocí klávesy S nebo kliknutím na tlačítko „Shoot“
-	hráč přijde o jeden život, jakmile se nepřítel dostane za modrou čáru, nepřítel umírá
-	pokud se za čáru dostane boss, hráč prohrává, i když má více než 1 život
-	bossové mohou náhodně přejít na jakoukoliv řadu po každé trefené střele, zachovají si ale svůj postup k hráči
-	hráč získává 20 skóre za každého zabitého nepřítele a 50 za bosse. Za každý ztracený život ztrátí 25 skóre
- racers mohou v řadě předběhnout ostatní nepřátele

