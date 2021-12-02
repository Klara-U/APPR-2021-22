# Analiza podatkov s programom R - 2021/22

Repozitorij z gradivi pri predmetu APPR v študijskem letu 2021/22

## Število ljudi z depresijo in ostalimi duševnimi motnjami v Evropi

Odkar smo v času korona krize je vse več govora o porastu depresije, anksioznosti ter ostalih duševnih motenj. Sedaj prav zagotovo to ni več takšna tabu tema kot je bila morda včasih. Pa tudi že pred korono se je precej govorilo o tem, predvsem v povezavi z razvitostjo držav in s tem povezanim pritiskom na posameznika glede njegove kariere ter v povezavi z družbenimi omrežji in primerjanjem z vrstniki. 

V tej analizi bi rada preverila razširjenost duševnih motenj(depresija, anksiozna motnja, bipolarna motnja, motnje prehranjevanja, shizofrenija, ADHD, obsesivno-kompulzivna motnja...) v evropskih državah, pri čemer bi rada še posebej primerjala razširjenost depresije. Primerjala bom razširjenost le-teh glede na starostno mediano, izobrazbeno sestavo, številom poročenih oseb, BDP-jem na osebo ter stopnjo urbanizacije države.

Delež ljudi z duševnimi motnjami bom primerjala tudi z številom zaposlenih v psihiatriji in deležem sredstev državnega proračuna, ki so namenjena pomoči ljudem z duševnimi težavami ter prikazala, kako se je delež ljudi z depresijo spreminjal skozi čas glede na rast BDP na prebivalca.

### Viri

* https://ec.europa.eu/eurostat/data/database - CSV, XLSX, HTML
* https://ourworldindata.org/ - CSV
* https://databank.worldbank.org/home.aspx - XLSX

### Tabele

Urejeni podatki se nahajajo v štirih razpredelnicah.
Vse meritve si bom ogledala za vsako evropsko državo posebej, 

1. tabela
* država, št. prebivalcev, mediana starosti prebivalcev, stopnja izobraženosti, št.ljudi v partnerskih zvezah, število ljudi z duševnimi motnjami, delež ljudi z depresijo
2. tabela
* država, delež ljudi z duševnimi motnjami, delež ljudi z depresijo, BDP per capita, stopnja urbanizacije
3. tabela 
* država, delež ljudi z duševnimi motnjami, št zaposlenih v psihiatriji, sredstva namenjena zdravljenju duševnih bolezni
4. tabela 
* država, leto, BDP per capita, delež ljudi z depresijo

## Program

Glavni program in poročilo se nahajata v datoteki `projekt.Rmd`.
Ko ga prevedemo, se izvedejo programi, ki ustrezajo drugi, tretji in četrti fazi projekta:

* obdelava, uvoz in čiščenje podatkov: `uvoz/uvoz.r`
* analiza in vizualizacija podatkov: `vizualizacija/vizualizacija.r`
* napredna analiza podatkov: `analiza/analiza.r`

Vnaprej pripravljene funkcije se nahajajo v datotekah v mapi `lib/`.
Potrebne knjižnice so v datoteki `lib/libraries.r`
Podatkovni viri so v mapi `podatki/`.
Zemljevidi v obliki SHP, ki jih program pobere,
se shranijo v mapo `../zemljevidi/` (torej izven mape projekta).