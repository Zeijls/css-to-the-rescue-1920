# CSS to the Rescue @cmda-minor-web 18-19

**Voor dit vak heb ik een interactieve menukaart gemaakt**

![Front-page](img/lightmode.png)

![Front-page](img/darkmode.png)

## Concept

## Leerproces

**CSS Animation Transform**
Als eerst ben ik begonnen met het laten bewegen van een SVG zodra er overheen wordt gehovert. Dit heb ik gedaan doormiddel van keyframes, transform:rotate en transform:translatey. Ik had hier nog nooit mee gewerkt, dus dit heeft me zeker op weg geholpen. Verder heb ik nog even verder gelezen over de andere mogelijkheden, en die wil ik nog een keer gaan uitproberen, maar nu achterwegen gelaten omdat er nog zoveel andere selectoren zijn. 

**Dark mode Switch button**
Switch button met toggle
Als eerst begon ik met een switch button maken, hier heb ik een toggle voor gebruikt en gestylt met een trasistion. 

Target Selector
Ik wist nog niet zo goed hoe ik het moest aanpakken om de darkmodus toe te passen. Ik had hiervoor Bas om hulp gevraagd, en hij gaf aan dat ik hier de target selector kon gebruiken. Hij gaf aan dat ik een ID kon zetten op de Header. En door deze ID aan te roepen in een link die ik om de switch button had heen gezet, zou ik vervolgens met :target#header ~ body {} de body aanroepen waarin de data werd veranderd. Dit werkte niet omdat er iets mis ging met de link. De link gaf geen groote, ook niet als ik deze een styling gaf. Ik heb hulp gevraagd aan May (Studentassistent) en die gaf aan dat de checkbox hack hier een betere oplossing voor is. Dit ben ik gaan uitzoeken. 

Checkbox hack
Toen ik de kleuren wilde aanpassen zodra de switch werd geselecteerd moest ik een checkbox hack gebruiken. Dit deed ik op de volgende manier: 
  input[type=checkbox]:checked ~ [full-background] {
        background-color: #AFC2DD;
  }

  input[type=checkbox]:checked ~ main .sun {
      display: none;
  }

  Het probleem was hiervoor dat de input type checkbox en de main niet dezelfde parent hadden. Dit kwam doordat er een div om de switch button heen zat, en de main hierbuiten viel. Hiervoor heb ik hulp gekregen van  Daan Ronger (Studentassistent). Hij gaf aan dat het divje waar de switchbutton in stond ook om de main moest staan om dit probleem op te lossen. 

  Tot hier heb ik mij vooral gericht op het concept, en aan de hand van wat ik nodig had voor het concept, heb ik nieuwe CSS selectors geleerd. Vanaf nu wil ik het andersom gaan gebruiken, en in de lijst van CSS selectoren kijken en het gewoon uitproberen.



***Bronnen***
[Target Selector](https://css-tricks.com/almanac/selectors/t/target/)
[Switch button Day/Night](https://codepen.io/AngelaVelasquez/pen/cihEG)
[Checkbox Hack](https://codepen.io/JiveDig/pen/jbdJXR/)

## Leerdoelen





