Zadání projektu 1
Cílem projektu je vyzkoušet si základní znalosti jazyka CSS, jednotlivých CSS pravidel a schopnost aplikovat různé typy CSS selektorů.

Stáhněte si archiv itw_proj1.zip a rozbalte. Archiv obsahuje:

soubor index.html reprezentující obsah a strukuturu webové prezentace fiktivní detektivní kanceláře,
adresář img/ obsahující použité ilustrace,
adresář css/ obsahující prázdný soubor style.css.
Implementujte soubor style.css bez nutnosti modifikace souboru index.html a přiložených obrázků tak, aby výsledná webová prezentace "pokud možno" odpovídala následujícím snímkům a popisu.

video
768px, 1200px, 1920px
pozn. #1: soubor index.html není žádané modifikovat, i když by se to v některých případech mohlo jevit jako smysluplnější řešení a v praxi byste tak pravděpodobně učinili; chápejte nicméně toto zadání spíše jako cvičení, v kterém si vyzkoušíte různé možnosti jazyka CSS (zejména práci s CSS selektory); možnost navrhnout si celou strukturu dle sebe dostanete v druhém projektu
pozn. #2: není nutné pracovat s přesností na pixely (bude hodnocena především znalost principů)
Všeobecné vlastnosti webové prezentace
šířka stránky se musí plynule přizpůsobit šířce okna prohlížeče:
minimální: 768px (při nižších velikostech je možné zobrazit horizontální scrollbar)
maximální: 1200px (při vyšších velikostech bude stránka zarovnána na střed okna prohlížeče)
levý a pravý odsazení stránky: 20px
horní, spodní odsazení sekce: 60px, 80px
použitá písma:
PT Sans - základní - věškerý text
Special Elite - logo
pozn.: soubor index.html již obsahuje import příslušných písem z Google Fonts
základní velikosti písem:
běžný text v odstavcích:
velikost písma (menší): 14px
velikost písma (větší): 18px
výška řádku: 1.7
nadpisy:
druhé úrovně (větší): 40px;
druhé úrovně (menší): 32px;
třetí úrovně: 24px;
základní použité barvy:
#898989: základní šedá
#bfbfbf: světlejší šedá
#4d4d4d: tmavší šedá
#f7f7f7: nevýrazná
black: výzazná
white: výrazná inverzní
steelblue: dekorace
zaoblelní: 5px
stín: 10px
doba animace: .5s
Některé výše zmíněné vlastnosti mohly být přetížené v jednotlivých částech dokumentu.

Specifické vlastnosti jednotlivých částí dokumentu
#header (záhlaví)
výška: velikost viewportu, ale minimálně 400px
menu:
horní okraj: 10px
logo:
písmo: 25px
vzdálenost mezi položkami menu: 10px
navigace:
písmo 13px
mezera mezi písmeny: .05em
vycpávka: 5px vertikální a 15px horizontálně
rámeček: 1px
hlavní nadpis:
písmo: 64px, white
odsazení zespodu a zleva: 20px
tlačítko Get started:
větší písmo
vycpávka: 20px
rámeček: 2px
zaoblení: 15px
hlavní nadpis spolu s tlačítkem umístěn v 2/3 záhlaví
#services
šířka karty: 300px
mezera mezi kartami: 40px
rámeček s ikonou:
velikost: 50px
vycpávka: 5px
čára rámečku: 1px
implementujte styly tak, aby bylo možné přidat další elementy .services-column
#about
velikost obrázku: 40%, 50% (po najetí kurzoru)
mezera mezi obrázkem a odstavcem: 40px (vertikální), 80px (horizontálně)
implementujte styly tak, aby bylo možné přidat další elementy .about-item a obrázky se pozicovaly střídavě na levou a pravou stranu
#team
karty mají stejnou šířku
mezera mezi kartami: 20px
#stats
karty mají stejnou šířku
maximální šířka karty: 300px
minimální mezera mezi kartami: 20px
velikost písma ikonky: 32px
#price
šířka tabulka: 80%
mezera mezi řádky 20px
vycpávka řádku: 20px
vycpávka tlačítka: 20px
#refs
karty mají stejnou šířku
maximální šířka karty: 400px
velikost obrázku: 60px
#contact
výška mapy: 400px
mezera mezi vstupními položkami: 20px
vycpávka vstupních položek: 10px
text nevalidního vstupu: red
barva tlačítka po najetí kurzorem: green 10: #footer
horní a spodní odsazení sekce: 40px
Vlastnosti, které nejsou výše specifikovány se pokuste odhadnout z uvedených snímků (není nutné, aby bylo na pixel přesné - viz. pozn. #2)

Odevzdání
Do IS VUT odevzdejte samostaný soubor style.css. Název souboru ponechte.

Datum odevzdání: 27. 3. 2022 (do nedělní půlnoci)
Hodnocení: max. 20 bodů
