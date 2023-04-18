# PR22_JL-NFZ-KP-MZ
# Analiza energetike v Sloveniji
## Projektna naloga pri predmetu Podatkovno rudarjenje

Pri projektu za predmet Podatkovno rudarjenje smo analizirali področje zaposlovanja v Sloveniji. Za to temo smo se odločili, ker nas zanima trend zaposlovanja, brezposelnosti in višina plač na slovenskem trgu skozi leta.
<br><br>
V času pisanja vmesnega poročila smo delno odgovorili na 2 od 3 vprašanj, bolj natančno, primerjali smo stopnjo revščine po spolu ter kako stopnja izobrazbe vpliva na stopno revščine (2. vprašanje) ter primerjali, kako se število prostih delovnih mest bolj drastično spreminja v določenih panogah kot v drugih (3. vprašanje).
<br><br>
Koda, uporabljena za odgovarjanje na vprašanja je dostopna v Jupyter notebook formatu v mapi "https://github.com/janljubic/PR22jlnfzkpmz/tree/main/analiza".
<br><br>
Preden smo začeli z analizo podatkovnih zbirk smo morali uvožene podatkovne zbirke, ki so bile v formatu .PX prebrati s pomočjo programa PX-Win. Prebrano datoteko smo nato shranili v format .csv, katerega smo lahko prebrali. Podatki so bili ločeni z ";", prav tako pa smo morali nadomestiti šumnike in celice označene z "N", odstraniti presledke v imenih vrstic, pretvoriti nize v tip integer...

### 1. Višina bruto in neto plače

TBD

### 2 Stopnja tveganja revščine po posameznih statističnih regijah

#### 2.1 Stopnja brezposelnosti med spoloma:

Pri tem vprašanju se posvečamo predvsem korelaciji med spolom, izobrazbo in pa brezposelnostjo. Pri začetnih analizah smo ugotovili, da je brezposelnost pri moških z osnovnošolsko izobrazbo višja od brezposelnosti pri ženskah z isto izobrazbo. Trenutno smo mnenja, da so te podatki nekoliko zavajujoči, saj moram še dodatno filtrirati podatke saj za določene parametre nimamo enakega števila vzrocev. 

#### 2.2 Stopnja brezposelnosti glede na statistično regijo

Pri tem vprašanju smo naleteli na težavo in sicer to, da so podatki, ki smo jih dobili rezdeljeni samo na 2 regije, ki sta vzhodna in zahodna slovenija. Podatke smo uredii in trenutno opazili, da je brezposelnost žensk v vzhodni sloveniji pada veliko hitreje kot v zahodni sloveniji oziroma da pada že dlje časa.


### 3. Trendi zaposlovanja na različnih področjih gospodarskih dejavnosti

Kot naše zadnje vprašanje pa smo hoteli ugotoviti, kako se spreminja trend zaposlovanja v razčličnih gospodarskih panogah, kot so na primer: rudarstvo, predelovalne dejavnosti, gradbeništvo, gostinstvo, informacijske in komunikacijske dejavnosti... ter kako je pandemija Covid-19 vplivala na razne panoge.

#### 3.1 Panoge, ki naraščajo/padajo v popularnosti

Prvo podvprašanje, ki si ga bomo postavili je katere panoge se povečujejo v obsegu ter iščejo novo delovno silo, ter katere zaradi 

#### 3.2 Covid-19 pandemija

Ena izmed stvari, ki jo bomo hoteli raziskati je, katere izmed panog gospodarstva so bile v smislu zaposlitve najbolj prizadete zaradi pandemije Covid-19. Vsi recimo vemo, da je bilo veliko panog prizadetih ter je bila stopnja odpuščanja zelo visoka (npr. gostinstvo), kar bi bilo najverjetneje tudi razvidno iz naših podatkov.



