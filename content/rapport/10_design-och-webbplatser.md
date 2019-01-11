Responsiv webbdesign
=======================

En webbplats måste fungera lika bra på alla enheter oavsett skärmstorlek. Därför är det viktigt att göra webbplatsen responsiv, d.v.s. att designen anpassar sig efter skärmstorleken. Därför har jag valt att analysera fyra olika webbplatser för att undersöka hur designen anpassar sig och vilka tekniker som används.


Urval
-----------------------
Jag har valt att genomföra undersökningen på fyra olika webbplatser som tillhör några av de största företagen i Sverige. De som jag har valt ut är: [ICA](https://www.ica.se/), [SJ](https://www.sj.se), [IKEA](https://www.ikea.com/se/sv/) och [Åhlens](https://www.ahlens.se/).


Metod
-----------------------
För att göra en avgränsning har jag valt att undersöka samtliga webbplatser vid tre olika ”breakpoints” – 375px, 768px och 1440px vilket representerar tre olika enheter (iPhone, iPad och laptop). Jag har valt att undersöka både hur designen rent visuellt anpassar sig efter olika skärmstorlekar samt tekniken bakom genom att studera CSS-koden i DevTools.

SJ
-----------------------
[FIGURE src="image/analysis/www.sj.se_1440.png?h=500" caption="SJ, 1440px"]  
Vid en skärmstorlek på 1440px består designen av fyra kolumner placerade i en container med mycket luft på sidorna. Container har en fast bredd på 1160px (vid min-width 1200px).  Kolumnerna har en relativ bredd på 25%.

[FIGURE src="image/analysis/www.sj.se_768.png?h=500" caption="SJ, 768px"]  
Vid en skärmstorlek på 768px består designen istället av två kolumner och navigeringsmenyn har dolts och ersatts av en meny-knapp och logotypen har blivit centrerad i header. Container har fortfarande en fast bredd, denna gång 740px (vid min-width 760px).

[FIGURE src="image/analysis/www.sj.se_375.png?h=500" caption="SJ, 375px"]  
Vid en skärmstorlek på 375px består designen endast av en kolumn, även de två input-fälten har blivit en kolumn och staplas nu på varandra. Varken container eller kolumn har någon angiven bredd, båda är block-element vilket gör att de fyller ut hela sidans bredd. Media queries saknas vilket tyder på att webbplatsen är designad med utgångspunkten ”mobile first”. Media queries dyker upp först vid min-width 760px.


ICA
-----------------------
[FIGURE src="image/analysis/www.ica.se_1440.png?h=500" caption="ICA, 1440px"]  
Vid en skärmstorlek på 1440px består designen av fyra alternativt sex kolumner placerade i en container med fast bredd på 1200px (vid min width 1024px). Designen bygger på tekniken flex-box och de olika kolumnerna har en relativ max-bredd. Navigeringsmenyn är enkel och består av olika ikoner och en hamburgermeny används.

[FIGURE src="image/analysis/www.ica.se_768.png?h=500" caption="ICA, 768px"]  
Vid en skärmstorlek på 768px har antalet kolumner minskat till två alternativt fyra stycken. Container har nu en relativ max-bredd på 100%, även kolumnerna har en relativ max-bredd.

[FIGURE src="image/analysis/www.ica.se_375.png?h=500" caption="ICA, 375px"]  Vid en skärmstorlek på 375px har antalet kolumner halverats ytterligare en gång. Media queries saknas vilket innebär att webbplatsen är designad med utgångspunkten mobile first. Media query dyker upp vid en bredd på 480px. Navigeringsmenyn har haft samma design samt innehåll vid alla tre storlekar.


Åhlens
-----------------------
[FIGURE src="image/analysis/www.ahlens.se_1440.png?h=500" caption="Åhlens, 1440px"]  
Vid en skärmstorlek på 1440px består designen av fyra alternativt sex kolumner. Container har en fast max-bredd på 1360px och padding på 20px (vid min width 1024px). Kolumnerna har en relativ bredd som beräknas med funktionen calc() och är inline-block vilket gör att de flödar efter varandra.

[FIGURE src="image/analysis/www.ahlens.se_768.png?h=500" caption="Åhlens, 768px"]  
Vid en skärmstorlek på 768px består designen fortfarande av samma antal kolumner. Container har samma max-width men med mindre padding. Kolumnerna har samma relativa bredd. Navigeringen är delvis ersatt med en hamburgermeny.

[FIGURE src="image/analysis/www.ahlens.se_375.png?h=500" caption="Åhlens, 375px"]  
Vid en skärmstorlek på 375px har antalet kolumner halverats. Ingen media query används på container. Vissa av kolumnerna har ersatts med "slick slider” som är en jQuery plugin. Vissa kolumner använder fortfarande relativ bredd.  Använder ramverket AngularJS samt jQuery plugin för att göra webbplatsen responsiv.


Handelsbanken
-----------------------
[FIGURE src="image/analysis/www.handelsbanken.se_1440.png?h=500" caption="Handelsbanken, 1440px"]
Vid en skärmstorlek på 1440px består designen av två till fyra kolumner. Container har både en relativ bredd på 100% och en fast max-width på 960px, container är centrerad på sidan och det är mycket luft på sidorna. Kolumnerna har en relativ bredd i procent (vid min-width 768px) och float-metoden används för att få kolumnerna att flöda bredvid varandra.

[FIGURE src="image/analysis/www.handelsbanken.se_768.png?h=500" caption="Handelsbanken, 768px"]
Vid en skärmstorlek på 768px ser designen i princip likadan ut, det är lika många kolumner men luft på sidorna av container har minskat. Container använder nu relativ bredd satt till 100% men padding gör att det blir luft på sidorna. I navigeringsmenyn har några länkar försvunnit och ersatts med dropbox-menyer.

[FIGURE src="image/analysis/www.handelsbanken.se_375.png?h=500" caption="Handelsbanken, 375px"]  
Vid en skärmstorlek på 375px har en större förändring skett i designen. Nu är det endast en kolumn och de ikoner som tidigare var placerade i fyra kolumner har ersatts med vanliga textlänkar placerade i en lista. Navigeringsmenyn har ersatts med en hamburgermeny. Kolumnerna har nu en bredd på 100% och media queries saknas vilket tyder på att webbplatsen är designad med utgångspunkten mobile first. Media queries dyker upp först när skärmen har en min-width på 768px.




Resultat och analys
-----------------------
Slutsatsen av denna undersökning är att det finns ett tydligt mönster hur designen anpassar sig efter skärmstorleken. Vid större skärmar, desktop, är det mycket whitespace och flera kolumner och att det sedan minskar i takt med att skärmstorleken minskar. Vid mindre skärmar byts även navigeringen ut mot en så kallad hamburgermeny. Men undersökningen visar även att det finns en mängd olika tekniker att tillämpa för att göra webbplatsen responsiv.

Alla förutom Åhlens använder i olika omfattning sig av media queries för att applicera andra CSS-regler för olika skärmstorlekar. Samtliga är utformade med utgångspunkten ”mobile first” vilket innebär att man börjar med att designa för mindre skärmar och sedan anpassar designen så att den även fungerar på större skärmar. En fördel med detta är att man blir tvungen att prioritera vilka delar och vilken information som är viktigast på webbplatsen och som därmed ska framhävas först.

För att enkelt få designen att anpassa sig efter olika skärmstorlekar används nästan uteslutande relativa bredder angivna i procent. Men för att få kontroll på layouten vid större skärmar används en fast bredd på container-elementen.

En annan viktigt aspekt är att även anpassa bilderna efter skärmstorleken. I det här utvalet använder Handelsbanken attributet srcset för att definiera olika storlekar och pixeldensitet vilket gör att bilden som visas på webbplatsen anpassar sig efter enheten. SJ och Åhlens använder javascript för att göra bilderna responsiva. ICA anpassar inte bildernas storlek efter enhet men tillämpar lazy loading vilket gör att alla bilder inte läses in på samma gång utan bara när de visas på skärmen.

Övrigt
-----------------------
Jag har gjort den här analysen på egen hand.
