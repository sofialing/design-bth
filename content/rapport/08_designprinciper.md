---
---
Tema: Designprinciper
=======================

Detta tema har jag valt att bygga från grunden för att ge det en helt annan känsla än temat baserat på designelement. Jag valde att fokusera på designprinciperna __kontrast__, __hierarki__, __perspektiv__ och __rörelse__.

####Kontrast####
Jag har strävat efter att skapa en design med många kontraster. Temat innehåller olika färg- och storlekskontraster:

* Svart text vs. vit bakgrund / Vit text vs. svart bakgrund
* Svart bakgrundsfärg till navigering och footer vs. vit bakgrundsfärg till "main content"
* Grön accentfärg samt flash-bild med stark grön färg vs. en annars färglös design
* Stora feta rubriker vs. liten och tunn brödtext

####Hierarki####
Användandet av olika storleks- och färgkontraster bidrar även till att skapa en hierarki i designen. Exempelvis har designen en stor flash-bild med en stor fet rubrik som blir en visuell ingång i webbplatsen. De olika storlekskontrasterna i designen bidrar till att rangordna innehållet, t.ex. är breadcrumbs och nästa/föregående-navigeringen inte lika viktigt som sidans huvudinnehåll och därför är deras teckenstorlek mindre än brödtexten. Likaså är sidebar och "table of content"-menyn inte lika viktig som huvudinnehållet och därför tar den bara upp 4 kolumner jämfört med 14 kolumner.

####Perspektiv####
Perspektiv har jag tillämpat genom att låta element överlappa varandra. Navigeringen har en fixed positionering högst upp på sidan vilket gör att den överlappar övrigt innehåll när man skrollar ner på sidan. Navigeringen har även en skuggning som förstärker det överlappande perspektivet.

Flash-bilden har en _fixed background-attachment_ vilket gör att det ser ut som om "main content" overlappar bilden när man skrollar på sidan. På likande sätt har jag även lagt samma bild i region-after-main, vilket gör intrycket att "main content" är placerad ovanpå bilden.

####Rörelse####
För att få in mer rörelse i designen har jag lagt till en hover-effect på länkarna i navigeringsmenyn. Effekten är gjort med transition för att få en mjukare rörelse, grunden till denna effect hittade jag på codepen men jag har justerat så att den ska passa in i designen.


Referenser
-----------------------
* [Cava: Design Elements & Principles](https://www.canva.com/learn/design-elements-principles/)
* [Wikipedia: Visual Design Elements and Principles](https://en.wikipedia.org/wiki/Visual_design_elements_and_principles)
* [Visual Literacy](https://dbwebb.se/article/vl.pdf)
* The principles of beautiful web design, Jason Beaird & James George.
