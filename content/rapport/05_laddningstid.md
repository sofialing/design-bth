---
---
Laddningstid
=======================

Detta är en analys av tre olika webbplatser och deras laddningstid och förbättringsåtgärder.


Urval
-----------------------

Jag har valt att analysera tre olika webbplatser inom samma kategori, organistioner inom natur- och djurskydd. De jag har valt är: [WWF](https://www.wwf.se/), [Djurens rätt](https://www.djurensratt.se/) och [World Animal Protection](https://www.worldanimalprotection.se/). WWF och World Animal Protection är internationella organisationer och jag har analyserat deras svenska webbplatser.


Metod
-----------------------

För att genomföra analysen har jag valt mig av Googles verktyg PageSpeed Insights som kontrollerar webbplatsernas prestanda på både mobil och desktop. Jag har även använt Devtools i Chrome och kontrollerat webbplatsernas laddningstiderna under fliken networks. Jag har analyserat värden från tre undersidor med liknande innehåll från respektive webbplats.

Rådatan är sammanställd i ett kalkylark som hittas [här](https://docs.google.com/spreadsheets/d/1GMJecjYkVZ1zh9OBeihEX7Z5uBjrxaeHNgsWVRLmIwg/edit?usp=sharing).


WWF
-----------------------
[FIGURE src="image/analysis/wwf.png?w=800"]

De sidor som jag undersökte på denna webbplats fick enligt PageSpeed ett dåligt resultat på mobil, ca 25-35 av 100 vilket räknas som en långsam webbsida. Däremot gav desktop ett bättre resultat, ca 93-98 av 100.

De förbättringar som kan göras är att använda bilder i ett modernare bildformat och i rätt storlek, startsidan i mobil skulle exempelvis få en uppskattad tidsbesparing på 7,95 s om ett modernare bildformat användes. För att snabba upp laddningstiden kan man även minska eller skjuta upp användningen av Javascript och CSS som blockerar renderingen av sidan, enligt min mätning i DevTools laddas 139 resurser in på startsidan. En annan åtgärd är att minifiera Javascript och CSS-filter vilket också minskar laddningstiden.


Djurens rätt
-----------------------
[FIGURE src="image/analysis/dr.png?w=800"]

De sidor som jag undersökte på denna webbplats fick enligt enligt PageSpeed ett mindre bra resultat på mobil, ca 48-57 av 100 vilket är precis på gränsen till att räknas som en långsam webbplats. Desktop gav ett bättre resultat, ca 98-99 av 100 och räknas då som en snabb webbplats.

Möjliga förbättringsåtgärder är att skjuta upp inläsningen av bilder som inte visas på skärmen, så kallad lazy loading, och att använda bilder i ett modernare bildformat och i rätt storlek.


World Animal Protection
-----------------------
[FIGURE src="image/analysis/wasp.png?w=800"]

De sidor som jag undersökte på denna webbplats fick enligt enligt PageSpeed ett hyfsat resultat på mobil, ca 70 av 100 vilket räknas som en genomsnittligt hastighet jämfört med andra webbplatser. Desktop gav ett toppresultat, och snittade på 99-100 av 100.

Möjliga förbättringsåtgärder är att ta bort resurser som exempelvis javascript och css som blockerar renderingen av sidorna samt att använda ett modernare bildformat och skjuta upp inläsningen av bilder som inte visas på skärmen. Javascript verkar inte vara minifierad, att göra det skulle även snabba upp laddningstiden.

Resultat
-----------------------
1. Word Animal Protection
2. Djurens rätt
3. WWF

Enligt mina mätningar har World Animal Protection den webbplats som presterar bäst när det gäller laddningstider, både på mobil och desktop. Den använder minst antal resurser och har minst totala storlek jämfört med de två andra. Enligt mina mätningar har WWF den webbplats som har sämst laddningstid, den använder överlägset mest resurser vilket ger en långsam laddningstid. Sidorna i mina mätningar har även störst totala storlek jämfört med WAP och Djurens rätt.
Det förvånade mig att WWF, som är en stor internationell organisation, har en så dåligt optimerad webbplats.

Sammanfattningsvis hade alla tre webbplatser liknande förbättringsåtgärder. Mycket handlar om bilder och att använda rätt storlek och format samt att tillämpa lazy loading, d.v.s. att skjuta upp inläsningen av bilder som inte visas på skärmen. Alla tre hade mer eller mindre problem med att resurser (t.ex. Javascript och CSS) blockar de första renderingarna av sidorna, detta åtgärdas exempelvis genom att dela upp och ta bort CSS-kod som inte används. Gemensamt för alla tre webbplatserna är att de är bättre optimerade för desktop än mobil.

Att sätta en absolut laddningstid tycker jag är svårt, det beror på enhet och uppkoppling. Men på en dator med snabbt internet så vill jag inte att det ska ta mer än några sekunder att läsa in en webbplats, så om en webbplats laddar i mer än 5 sekunder skulle jag nog betrakta den som långsam. Jag använder mest mobil när jag besöker webbplatser och då kan jag acceptera att det tar något längre tid, dock önskar jag att fler blev bättre på att optimera sina webbplatser så att de laddar snabbare på mobilen.


Referenser
-----------------------
* [PageSpeed Insight](https://developers.google.com/speed/pagespeed/insights/)
* [Moz Page Speed](https://moz.com/learn/seo/page-speed)
* [PageSpeed Insights Rules](https://developers.google.com/speed/docs/insights/rules)

Övrigt
-----------------------
Jag har gjort den här analysen på egen hand.
