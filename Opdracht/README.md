# CSS to the Rescue @cmda-minor-web 18-19

**Voor dit vak heb ik een interactieve menukaart gemaakt**

![Front-page](img/lightmode.png)

![Front-page](img/darkmode.png)

## Keuze opdracht

**Choose one asignment**
- [x] Responsive restauraunt menu Here’s some raw HTML you may use
- [ ] One art directed responsive web page for a magazine on the web. Here’s some example HTML
- [ ] Have a better idea? Nice! Pitch it to us.

**Context**
You have to add at least one extra context to your site

- [ ] Print-stylesheet
- [ ] Prefers-reduced-motion
- [x] Dark-mode
- [ ] Input type (pointer)
- [ ] <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries">pick a better one</a>


**Pick two restrictions**
You have to work with _at least_ two of these restrictions.

- [x] When SVG meets CSS: Shapes / Masks / SVG
- [ ] Two colours
- [ ] Less than 5kb CSS *(not as an excuses for lazyness, hahaha)*
- [ ] No squares, no rectangles, no circles, no triangles
- [ ] Design must be visually appealing and it must meet <a href="https://www.w3.org/TR/WCAG20/#guidelines">Level AAA conformance</a> of the WCAG.
- [ ] Solar powered website
- [ ] Responsive without media queries
- [ ] Design responds to weather/time
- [ ] Design responds to connectivity
- [ ] Design responds to battery level
- [ ] Design responds to language setting
- [ ] Design responding language setting / Japanese / English / Greek / Mongolian
- [ ] Create a great experience only with pop-ups, advertising banners and carousels!

**The *Selector First* CSS Methodology**

You _have_ to work with the so called *Selector First* CSS Methodology. This means that you _have to_ use a wide variety of CSS selectors. ID’s are only allowed to trigger the `:target` selector. If you really need them, you are allowed to use a few classes. In order to differentiate between 

## Leerdoelen
- You understand the broader scope of CSS: You can show that CSS can be used for more than just styling web pages.
- You understand the progressive enhancement parts of CSS: You can show that you can use the cascade, inheritance and specificity in your project
- You understand the interactive parts of CSS: Is the UX fully enhanced within in given CSS scope?
- You have been experimenting: Have the learning goals been stretched?

## Concept

## Leerproces

### Readme Opstellen
Als eerst moest ik deze readme opstellen, ik zag bij andere dat ze kopjes, linkjes en takenlijsten gebruikten. Ik had geen idee dus ik ben het volgende artikel gaan lezen en uitproberen.

***Bron*** 
[Basic writing and formatting syntax ](https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax#paragraphs)

### CSS Animation Transform
Ik ben begonnen met het laten bewegen van een SVG zodra er overheen wordt gehovert. Dit heb ik gedaan doormiddel van keyframes, transform:rotate en transform:translatey. Ik had hier nog nooit mee gewerkt, dus dit heeft me zeker op weg geholpen. Verder heb ik nog even verder gelezen over de andere mogelijkheden, en die wil ik nog een keer gaan uitproberen, maar nu achterwegen gelaten omdat er nog zoveel andere selectoren zijn. 

***Bron*** 
[CSS Animation](https://css-tricks.com/almanac/properties/a/animation/)

### Dark mode Switch button
Switch button met toggle
Als eerst begon ik met een switch button maken, hier heb ik een toggle voor gebruikt en gestylt met een trasistion. 

***Bron***
[Switch button Day/Night](https://codepen.io/AngelaVelasquez/pen/cihEG)

### Target Selector
Ik wist nog niet zo goed hoe ik het moest aanpakken om de darkmodus toe te passen. Ik had hiervoor Bas om hulp gevraagd, en hij gaf aan dat ik hier de target selector kon gebruiken. Hij gaf aan dat ik een ID kon zetten op de Header. En door deze ID aan te roepen in een link die ik om de switch button had heen gezet, zou ik vervolgens met :target#header ~ body {} de body aanroepen waarin de data werd veranderd. Dit werkte niet omdat er iets mis ging met de link. De link gaf geen groote, ook niet als ik deze een styling gaf. Ik heb hulp gevraagd aan May (Studentassistent) en die gaf aan dat de checkbox hack hier een betere oplossing voor is. Dit ben ik gaan uitzoeken. 

I'd use these rules-of-thumb for when :target is a good choice:

When a "state" is needed
When the jump-down/hash-link behavior is acceptable
When it's acceptable to affect the browser history

***Bron*** 
[Target Selector](https://css-tricks.com/almanac/selectors/t/target/)

### Checkbox hack
Toen ik de kleuren wilde aanpassen zodra de switch werd geselecteerd moest ik een checkbox hack gebruiken. Dit deed ik op de volgende manier: 
    
    input[type=checkbox]:checked ~ [full-background] {
        background-color: #AFC2DD;}

    input[type=checkbox]:checked ~ main .sun {
        display: none;}  

  Het probleem was hiervoor dat de input type checkbox en de main niet dezelfde parent hadden. Dit kwam doordat er een div om de switch button heen zat, en de main hierbuiten viel. Hiervoor heb ik hulp gekregen van  Daan Ronger (Studentassistent). Hij gaf aan dat het divje waar de switchbutton in stond ook om de main moest staan om dit probleem op te lossen.   

  Tot hier heb ik mij vooral gericht op het concept, en aan de hand van wat ik nodig had voor het concept, heb ik nieuwe CSS selectors geleerd. Vanaf nu wil ik het andersom gaan gebruiken, en in de lijst van CSS selectoren kijken en het gewoon uitproberen.  

***Bron*** 
[Checkbox Hack](https://codepen.io/JiveDig/pen/jbdJXR/)

## Takenlijst
- [ ] Concept schrijven
- [x] Readme Opstellen
- [x] Criteria doorlezen
- [ ] Nog een ristrictie uitwerken
- [ ] Geen classes
- [ ] Responsive maken
- [ ] Readme bijwerken




