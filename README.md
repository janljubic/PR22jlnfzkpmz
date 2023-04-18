@@ -1 +1,104 @@
# PR22_JL-NFZ-KP-MZ
# Analiza energetike v Sloveniji
## Projektna naloga pri predmetu Podatkovno rudarjenje

Pri projektu za predmet Podatkovno rudarjenje smo analizirali področje zaposlovanja v Sloveniji. Za to temo smo se odločili, ker nas zanima trend zaposlovanja, brezposelnosti in višina plač na slovenskem trgu skozi leta.
<br><br>
V času pisanja vmesnega poročila smo delno odgovorili na 2 od 3 vprašanj, bolj natančno, primerjali smo stopnjo revščine po spolu ter kako stopnja izobrazbe vpliva na stopno revščine (2. vprašanje) ter primerjali, kako se število prostih delovnih mest bolj drastično spreminja v določenih panogah kot v drugih (3. vprašanje).
<br><br>
Koda, uporabljena za odgovarjanje na vprašanja je dostopna v Jupyter notebook formatu v mapi "https://github.com/janljubic/PR22jlnfzkpmz/tree/main/analiza".


## 1. Višina bruto in neto plače

TBD


### 2 Stopnja tveganja revščine po posameznih statističnih regijah




### 2.2 Iskanje korelacije v podatkih

Nato smo želeli najti potencialne odvisnosti v ceni različnih energentov. To smo storili tako da smo najprej zračunali pearsonove koeficiente korelacije ter p-vrednosti za kombinacije atributov podatkovne množice, ki so se nam zdeli smiselni oziroma zanimivi.
<br><br>
Pri tem smo ugotovili, da cene pogonskih goriv, kurilnega olja in zemeljskega plina korelirajo, kar je smiselno, saj gre za energente, ki spadajo v skupino foslinih goriv. Bencin, dizel in pa kurilno olje se pridobivajo iz nafte zato njihova cena seveda močno korelira (bencin in dizel imata pearsonov koeficient korelacije 0.90, dizel in kurilno olje pa 0.93) in je verjetno tudi močno odvisna od cene nafte.
<br><br> 
Prav tako smo ugotovili, da cene pogonskih goriv in električne energije ne korelirajo v primeru gospodinjskih odjemalcev, pač pa korelirajo v primeru negospodinjskih odjemalcev (pearsonov koeficietn korelacije je namreč 0.61). Sklepamo da, zato ker se pogonska goriva ne uporabljajo pri proizvodnji električne energije ali ogrevanju (z izjemo kurilnega olja, kar pa ne spremeni rezultatov, saj je pearsonov koeficient korelacije cene olja in električne energije gospodinjskih odjemalcev 0.064).
<br><br>
Ugotovili smo tudi, da cene zemeljskega plina in električne energije pri negospodinjskih odjemalcih korelirajo (pearsonov koeficient korelacije ima vrednost 0.72), pri negospodinjskih pa ne (pearsonov koeficient korelacije ima vrednost -0.14). Sklepamo da je razlog zato, uporaba zemeljskega plina pri proizvodnji električne energije.
<br><br>
Zanimivo se nam je zdelo da cene električne energije pri gospodinjskih in negospodinjskih odjemalcih ne korelirajo (pearsonov koeficient korelacije ima vrednost -0.14), cene zemeljskega plina pri gospodinjskih in negospodinjskih odjemalcih pa vendar korelirajo (pearsonov koeficient korelacije je 0.77).
<br>

#### 2.2.1 Grafičen prikaz nekaterih ugotovitev

Z uporabo razsevnih diagramov, kjer vsaka točka predstavlja četrtletje smo primerjali odvisnosti cen po dveh energentov. Zelena diagonala na diagramih predstavlja pozitivno korelacijo cen energentov, rdeča pa negativno. Pri diagramih v katerih sta narisani obe diagonali, sta te predstavljeni z razlogom prikaza, da se cene ne korelirajo po nobeni od njiju. Na tak način smo dodatno potrdili zgornje ugotovitve ter jih vizualno predstavili [(vsi grafi so na voljo v zvezku fuel_correlation.ipynb)](src/fuel_correlation.ipynb).
<br>
![Prva točka](resources/Korelacija%201.png) ![Druga točka](resources/Korelacija%202.png)

# Razlaga strukture direktorija naloge
## analiza
- vsebuje vse pripadajoče Jupyter datoteke, ki se navezujejo na obdelavo in analizo podatkovnih virov.
- različni predmeti analize, ki tematsko predstavljajo celoto, so združeni v poddirektorije.
## dokumenti
- vsi relevantni dokumenti, ki se uporabljajo v procesu odkrivanja uporabnih znanj o podatkovnih virih, ki smo jih tekom naloge uporabili - predvsem so ključnega pomena metodološka pojasnila.
## podatki
- vse datoteke z uporabljenimi podatki.
- datoteke, katerih imena se začenjajo z 'original_file', predstavljajo prvotno .px datoteko, ki smo jo pridobili.
- datoteke, katerih imena se začenjajo s 'filtered', predstavljajo urejeno in filtrirano .csv datoteko (DOKONČNA TRANSFORMACIJA).
- preostale datoteke predstavljajo .csv datoteke, ki smo jih pridobili po transformaciji iz .px datoteke.
## PX-Win
- statistično orodje, ki se uporablja za obravnavo .px datotek.
## slike
- pripadajoče vizualizacije in razno slikovno gradivo.
