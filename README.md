
<!DOCTYPE html>
<html lang="cs">

<head>
    <meta http-equiv="content-type" content="text/html; charset=utf-8" />
    <title>Tvorba webových stránek - Projekt 1</title>
    <link rel="stylesheet" type="text/css" href="../../itw.css">
    <style>
        img {
            border: 1px solid #eee;
            padding: 0.5em;
            margin: 1em 0;
        }
    </style>
</head>

<body>

    <h1>Tvorba webových stránek</h1>
    <div class="kontakt">
    </div>

    <div class="menu">
        <h2>Materiály k předmětu</h2>
        <ul>
            <li><a href="../../prednasky/.cs">Přednášky (slajdy)</a></li>
            <li><a href="../../cviceni/.cs">Materiály ke cvičení</a></li>
            <li><a href="../../kontakt.html.cs">Konzultace a kontakt</a></li>
        </ul>
        <hr />
        <ul>
            <li><a href="../../index.html.cs">Úvod</a></li>
        </ul>
    </div>

    <div class="contentbox">

            <h2>Zadání projektu 1</h2>
            <p>Cílem projektu je vyzkoušet si základní znalosti jazyka CSS, jednotlivých CSS pravidel a schopnost aplikovat
                různé typy CSS selektorů.</p>
            <ol>
                <li>
                    <p>Stáhněte si archiv <a href="files/itw_proj1.zip"><code>itw_proj1.zip</code></a> a rozbalte. Archiv
                        obsahuje:</p>
                    <ol>
                        <li>soubor <code>index.html</code> reprezentující obsah a strukuturu webové prezentace fiktivní
                            detektivní kanceláře,</li>
                        <li>adresář <code>img/</code> obsahující použité ilustrace,</li>
                        <li>adresář <code>css/</code> obsahující prázdný soubor style.css.</li>
                    </ol>
                </li>
                <li>
                    <p>Implementujte soubor <code>style.css</code> bez nutnosti modifikace souboru <code>index.html</code> a
                        přiložených obrázků tak, aby výsledná webová prezentace &quot;pokud možno&quot; odpovídala následujícím
                        snímkům a popisu.</p>
                    <ul>
                        <li><a href="https://drive.google.com/file/d/1jGOSCwlJ-cNXzlN_erAPZQghm_b1rFeX/view?usp=sharing">video</a>
                        </li>
                        <li><a href="files/768px.png">768px</a>, <a href="files/1200px.png">1200px</a>, 
                            <a href="files/1920px.png">1920px</a></li>
                        <li>pozn. #1: soubor <code>index.html</code> není žádané modifikovat, i když by se to v některých
                            případech mohlo jevit jako smysluplnější řešení a v praxi byste tak pravděpodobně učinili; chápejte
                            nicméně toto zadání spíše jako cvičení, v kterém si vyzkoušíte různé možnosti jazyka CSS (zejména
                            práci s CSS selektory); možnost navrhnout si celou strukturu dle sebe dostanete v druhém projektu
                        </li>
                        <li>pozn. #2: není nutné pracovat s přesností na pixely (bude hodnocena především znalost principů)</li>
                    </ul>
                </li>
            </ol>
            <h3 id="vseobecne">Všeobecné vlastnosti webové prezentace</h3>
            <ul>
                <li>šířka stránky se musí plynule přizpůsobit šířce okna prohlížeče:<ul>
                        <li>minimální: <code>768px</code> (při nižších velikostech je možné zobrazit horizontální scrollbar)
                        </li>
                        <li>maximální: <code>1200px</code> (při vyšších velikostech bude stránka zarovnána na střed okna
                            prohlížeče)</li>
                    </ul>
                </li>
                <li>levý a pravý odsazení stránky: <code>20px</code></li>
                <li>horní, spodní odsazení sekce: <code>60px</code>, <code>80px</code></li>
                <li>použitá písma:<ol>
                        <li><code>PT Sans</code> - základní - věškerý text</li>
                        <li><code>Special Elite</code> - logo</li>
                        <li>pozn.: soubor <code>index.html</code> již obsahuje import příslušných písem z <a
                                href="https://fonts.google.com/">Google Fonts</a></li>
                    </ol>
                </li>
                <li>základní velikosti písem:<ul>
                        <li>běžný text v odstavcích:<ul>
                                <li>velikost písma (menší): <code>14px</code></li>
                                <li>velikost písma (větší): <code>18px</code></li>
                                <li>výška řádku: <code>1.7</code></li>
                            </ul>
                        </li>
                        <li>nadpisy:<ul>
                                <li>druhé úrovně (větší): <code>40px</code>;</li>
                                <li>druhé úrovně (menší): <code>32px</code>;</li>
                                <li>třetí úrovně: <code>24px</code>;</li>
                            </ul>
                        </li>
                    </ul>
                </li>
                <li>základní použité barvy:<ul>
                        <li><code>#898989</code>: základní šedá</li>
                        <li><code>#bfbfbf</code>: světlejší šedá</li>
                        <li><code>#4d4d4d</code>: tmavší šedá</li>
                        <li><code>#f7f7f7</code>: nevýrazná</li>
                        <li><code>black</code>: výzazná</li>
                        <li><code>white</code>: výrazná inverzní</li>
                        <li><code>steelblue</code>: dekorace</li>
                    </ul>
                </li>
                <li>zaoblelní: <code>5px</code></li>
                <li>stín: <code>10px</code></li>
                <li>doba animace: <code>.5s</code></li>
            </ul>
            <p>Některé výše zmíněné vlastnosti mohly být přetížené v jednotlivých částech dokumentu.</p>
            <h3 id="specificke">Specifické vlastnosti jednotlivých částí dokumentu</h3>
            <ol>
                <li><code>#header</code> (záhlaví)<ul>
                        <li>výška: velikost viewportu, ale minimálně <code>400px</code></li>
                        <li>menu:<ul>
                                <li>horní okraj: <code>10px</code></li>
                                <li>logo:<ul>
                                        <li>písmo: <code>25px</code></li>
                                    </ul>
                                </li>
                                <li>vzdálenost mezi položkami menu: <code>10px</code></li>
                                <li>navigace:<ul>
                                        <li>písmo <code>13px</code></li>
                                        <li>mezera mezi písmeny: <code>.05em</code></li>
                                        <li>vycpávka: <code>5px</code> vertikální a <code>15px</code> horizontálně</li>
                                        <li>rámeček: <code>1px</code></li>
                                    </ul>
                                </li>
                            </ul>
                        </li>
                        <li>hlavní nadpis:<ul>
                                <li>písmo: <code>64px</code>, <code>white</code></li>
                                <li>odsazení zespodu a zleva: <code>20px</code></li>
                            </ul>
                        </li>
                        <li>tlačítko <em>Get started</em>:<ul>
                                <li>větší písmo</li>
                                <li>vycpávka: <code>20px</code></li>
                                <li>rámeček: <code>2px</code></li>
                                <li>zaoblení: <code>15px</code></li>
                            </ul>
                        </li>
                        <li>hlavní nadpis spolu s tlačítkem umístěn v 2/3 záhlaví</li>
                    </ul>
                </li>
                <li><code>#services</code>
                    <ul>
                        <li>šířka karty: <code>300px</code></li>
                        <li>mezera mezi kartami: <code>40px</code></li>
                        <li>rámeček s ikonou:<ul>
                                <li>velikost: <code>50px</code></li>
                                <li>vycpávka: <code>5px</code></li>
                                <li>čára rámečku: <code>1px</code></li>
                            </ul>
                        </li>
                        <li>implementujte styly tak, aby bylo možné přidat další elementy <code>.services-column</code></li>
                    </ul>
                </li>
                <li><code>#about</code>
                    <ul>
                        <li>velikost obrázku: <code>40%</code>, <code>50%</code> (po najetí kurzoru)</li>
                        <li>mezera mezi obrázkem a odstavcem: <code>40px</code> (vertikální), <code>80px</code> (horizontálně)
                        </li>
                        <li>implementujte styly tak, aby bylo možné přidat další elementy <code>.about-item</code> a obrázky se
                            pozicovaly střídavě na levou a pravou stranu</li>
                    </ul>
                </li>
                <li><code>#team</code>
                    <ul>
                        <li>karty mají stejnou šířku</li>
                        <li>mezera mezi kartami: <code>20px</code></li>
                    </ul>
                </li>
                <li><code>#stats</code>
                    <ul>
                        <li>karty mají stejnou šířku</li>
                        <li>maximální šířka karty: <code>300px</code></li>
                        <li>minimální mezera mezi kartami: <code>20px</code></li>
                        <li>velikost písma ikonky: <code>32px</code></li>
                    </ul>
                </li>
                <li><code>#price</code>
                    <ul>
                        <li>šířka tabulka: <code>80%</code></li>
                        <li>mezera mezi řádky <code>20px</code></li>
                        <li>vycpávka řádku: <code>20px</code></li>
                        <li>vycpávka tlačítka: <code>20px</code></li>
                    </ul>
                </li>
                <li><code>#refs</code>
                    <ul>
                        <li>karty mají stejnou šířku</li>
                        <li>maximální šířka karty: <code>400px</code></li>
                        <li>velikost obrázku: <code>60px</code></li>
                    </ul>
                </li>
                <li><code>#contact</code>
                    <ul>
                        <li>výška mapy: <code>400px</code></li>
                        <li>mezera mezi vstupními položkami: <code>20px</code></li>
                        <li>vycpávka vstupních položek: <code>10px</code></li>
                        <li>text nevalidního vstupu: <code>red</code></li>
                        <li>barva tlačítka po najetí kurzorem: <code>green</code>
                            10: <code>#footer</code></li>
                        <li>horní a spodní odsazení sekce: <code>40px</code></li>
                    </ul>
                </li>
            </ol>
            <p>Vlastnosti, které nejsou výše specifikovány se pokuste odhadnout z uvedených snímků (není nutné, aby bylo na pixel přesné - viz. pozn. #2)</p>
            <h3 id="odevzdani">Odevzdání</h3>
            <p>Do IS VUT odevzdejte samostaný soubor <code>style.css</code>. Název souboru ponechte.</p>
            <p><strong>Datum odevzdání:</strong> 27. 3. 2022 (do nedělní půlnoci)<br>
                <strong>Hodnocení:</strong> max. 20 bodů
            </p>
    </div>

</body>

</html>
