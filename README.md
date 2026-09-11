# Sematisk HTML:

Innebär att man utifrån innehållets betydelse väljer rätt typ av tagg, 
detta för att det ska vara mer enkelt för en skärmläsare att läsa av koden, 
istället för att det bara ska se bra ut visuellt, 
samt enklare för sökmotorer (SEO) att tolka vilken typ av hemsida det är.
Vi har valt att använda det på vår eventsida för att det skapar mer struktur i koden 
och gör det enklare att navigera sig runt, Det framstår tydligt vad som gör vad i koden.
För oss som utvecklare blir det enklare att förstå koden och felsöka den
när det finns beskrivande namn istället för att ha allt i div.

Exempel från vår kod: är bla. <main> och de följande <section> med dens egna underkategori <article> mm



# CSS Flexbox & CSS Grid

## CSS Flexbox
Flexbox är endimensionell layout system som gör det enklare att anpassa
utseendet och samtidigt få en responsiv layout med hjälp av flexbox egenskaper
Flexbox är bra om man vill ha object på en rad, som standard ligger det på rad
och man kan ändra riktning till columner med hjälp av flex-direction.

Ett bra exempel är .nav som gör att <li> elementen inte staplas vertikalt (vilket är standard annars) och med display: flex lägger vi dom på rad med gap: 1rem som mellanrum


## CSS Grid
Grid är tvådimensionell layout, det vill säga du kan ha både rader och kolumner,
är ett bra verktyg om man ska bland annat ska schema eller tabell, du kan enkelt
enkelt välja hur många columner du ska använda och hur stor bråkdel av hemsidan 
de ska ta genom att använda grid-template-columnns tex 1fr 2fr 2fr. 
då får man 1 mindre del och 2 större del, (fr står för fraction)

Motivering från vår egna kod där vi har använt CSS Grid är
på vårt <article class="Schema"> där vi har använt Grid för att skapa 
rutnät som är ett schema för de olika artister, vilka scener de spelar på
och öppettider i matkiosken. Vi använde Grid-template-columns: 1fr 1fr för att skapa
två columner och sedan i media queries har vi gjort att det blir till en column
med grid-template-columns: 1fr;
Detta gjorde att informationen är tydlig och i struktur så att det blir lätt att läsa.
samt anpassar layouten sig efter skärmbredd.



## CSS arv:
Betyder att vissa egenskaper hos föräldrer ärvs utav barnen, tillexempel color eller font-family, 
men det kan brytas om barnet definerar egenskapen själv