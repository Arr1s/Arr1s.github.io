# CSS to the Rescue
Voor CSS to the Rescue heb ik gekozen voor de film timeline opdracht met als film Inception. 

## Week 1
In de eerste week was het voornamelijk een concept bedenken, de grootste challenges eruit vissen en kijken welke verschillende types code ik kon gebruiken om deze challenges aan te gaan. 
### Concept
Mijn concept is om de timeline van Inception met 3D en layers van "dromen" per character te laten zien terwijl je hun kan volgen door de timeline heen. Je ziet dan welke layers ze ingaan, waar mensen splitsen en wat de grootste momenten waren (gevisualiseerd) op de verschillende niveau's kwa dromen. 

Mijn plan is om eerste in 2D te beginnen met een de hoofdkarakter, en denk dat als ik die helemaal af heb, het goed te doen moet zijn om de rest toe te voegen, met als nog een grote eind uitdaging het 3D maken.

Inspiratie:

<img width="256" alt="" src="https://github.com/user-attachments/assets/ba2c8150-9aa8-4571-a484-52566eb7d24c" />


Hierbij mijn eerste twee schetsen:

<img width="256" alt="" src="https://github.com/user-attachments/assets/e6762a75-4369-4bfc-9cf5-8a9c4ecbcac2" />
<img width="256" alt="" src="https://github.com/user-attachments/assets/2e14eea4-802c-4c17-849d-389157b6c935" />



### Proces
Ik heb mijn concept dus rond weten te krijgen, en heb ik een kleine start gemaakt met de code. Eerst was mijn plan om een gestylde div over een SVG heen te leggen en dan met VH en VW te animeren om hem responsive te houden, echter ging dit alles behalve volgens plan. Toen dacht ik dat misschien in plaats van VH en VW te gebruiken, ik de coördinaten uit de SVG kon overnemen, wat eerst goed leek te werken, maar uiteindelijk toch een beetje de soep in liep. Daarna kwam ik op het idee om twee SVG's over elkaar heen te leggen, en vervolgens beide met  over elkaar te laten liggen, en met *strokedashoffset* ze de lijn te laten tekenen. Echter ging dit opnieuw niet volgens plan, en ben ik uiteindelijk aangeraden om naar *motion-path* te kijken, wat ik van plan ben volgende week verder te onderzoeken en uit te werken. 

<img width="256" alt="Poging om met coors/vh en vw de div het juiste pad te laten volgen" src="https://github.com/user-attachments/assets/12f39b87-4c79-4a15-93f8-91440ead8079" />
<img width="385" alt="Poging om met de lijn zichzelf te laten tekenen" src="https://github.com/user-attachments/assets/56b0968c-c8f3-48ea-8733-df2bcd6a3ef8" />


### Conclusie
Ik ben aardig onderweg... denk ik... hoop ik... 

## Week 2

### Proces
Deze week ben ik met behoorlijk veel bezig geweest, ik heb de paden werkend gekregen, wat uiteindelijk een stuk sneller en makkelijker ging dan verwacht. Na de SVG over elkaar gezet te hebben, en de tweede SVG met een stroke-width groter gemaakt te hebben, en de stroke-linecap (uiteindes) op rond gezet te hebben werkte het helemaal naar behoren. Daarna ben ik verder gegaan met de info van inception erin te zetten ben ik verder gegaan met custom font toe te voegen en een kleine animatie hierbij te schrijven.

Toen had ik het idee om de andere tijdlijnen van de personages toe te voegen, en deze gebaseerd op het droom niveau waar ze achter werden gelatan af te laten snijden, om bij het einde weer bij elkaar te komen. Ik was eerst van plan om de eerste SVG simpelweg in illustrator aan te passen en deze dan toe te voegen en te laten overlappen, maar om de een of andere reden ging dat helemaal mis. Hij was kleiner dan de orginele, maar als ik hem dan schaalde bleek de offset van bepaalde lijnen ook niet meer te kloppen. Wat ik ook probeerde de SVG kon gewoon niet goed overlappen, dus ben ik maar de code van de eerste SVG gaan kopieren en heb toen hiervan handmatig te coordinaten aangepast. 

<img width="917" alt="Screenshot 2025-03-04 at 11 01 01" src="https://github.com/user-attachments/assets/1024bb61-8698-42d7-82d7-cda31ad2519d" />

Hierna was ik begonnen met proberen de lijnen in 3D te zetten, maar dit begon vrij veel met de verhouding van de lijnen te schuiven, dus besloot ik dat nog maar even links te laten liggen en op een later punt daarop terug te komen.

### Conclusie
- Betere styling, fonts per niveau aanpassen gebaseerd op droom, lijnen 3D maken

## Week 3

### Proces
Fonts toegevoegd, Grid toegevoegd met les van Nils.
Mijn eerste oplossing was om een RotateY(45deg) te maken, daarna met een transform op alle SVG's individueel apart te zetten, en daarna met een ScaleX(1.4) voor de breedte te compenseren. Echter bracht dit vele performance issues mee, en kwam Nils Binder uiteindelijk met A, een betere symmantisch, perfomance en visuele manier van de 3D lijnen.
Perspective op de section gestopt, want zonder section kan je geen 3D transform maken. Een rotateY(4deg) op de SVG's gestopt en de trasnforms laten staan. Debug werkt niet helemaal, toen van alle SVG's dezelfde paths in dezelfde SVG gestopt. Daarnaast een "pathLength" toegevoegd, daarmee kan je eigenlijk zeggen, deze lijn die in werkelijkheid 1357 pixels is, staat nu gelijk aan 100. Dit hielp met alle berekeningen van zowel de path als de custom properties te vereenvoudigen. 
gridtemplate
image proberen, pattern, image los, animateMotion, animateTransform,

Fonts die toegevoegd zijn met Wakamai Fondue
<img width="1470" alt="Screenshot 2025-03-10 at 15 15 51" src="https://github.com/user-attachments/assets/4566e403-c1d9-4c02-889a-0c4180879004" />

Grid toevoegingen aan m'n articels en deze proberen responsive te maken, wat niet al te best ging tot ik container queries ging gebruiken
<img width="1470" alt="Screenshot 2025-03-10 at 13 05 30" src="https://github.com/user-attachments/assets/454c7eaa-c144-46b3-8207-e8ba3561efa1" />
<img width="1470" alt="Screenshot 2025-03-10 at 13 05 18" src="https://github.com/user-attachments/assets/b954fd6b-37f0-4f68-8a7e-5cca83dd5c67" />
<img width="1470" alt="Screenshot 2025-03-10 at 13 05 37" src="https://github.com/user-attachments/assets/ab8a79d8-5e46-4d02-a455-a87830cc950d" />
<img width="1470" alt="Screenshot 2025-03-10 at 15 16 14" src="https://github.com/user-attachments/assets/668f4e7c-2e6a-4145-bd65-a58cf3a6322a" />

Container queries gebruiken met grid om het article wel responsive te maken met de gewenste layout
<img width="1470" alt="Screenshot 2025-03-17 at 12 50 20" src="https://github.com/user-attachments/assets/bfeb48e9-8940-4621-8a11-91c5f8759898" />


Gefaald experiment om een pad aan een plaatje te koppelen
<img width="1470" alt="Screenshot 2025-03-17 at 11 14 45" src="https://github.com/user-attachments/assets/e65a9cc5-8cd2-404d-bead-98def48452b9" />
![Poging image pad ](https://github.com/user-attachments/assets/5a8d655f-870c-42cc-948c-a28b5ab4ce90)
![poging image pad 2](https://github.com/user-attachments/assets/9031b7a8-51c9-4010-8e2f-bd92526a3bf3)
![poging alle image paden](https://github.com/user-attachments/assets/a54ab13a-c191-4bac-a295-2b75395d439d)


### Conclusie
De content is nu nog wel erg hektisch, ik zal een manier moeten vinden om A, de content gebaseerd op de lijnen nog responsive te houden, terwijl B, de content overzichtelijker wordt zodat het prettiger is om naar te kijken.

## Week 4
In week 4 heb ik gekeken naar de nesting van CSS elementen en deze meer doorgevoerd zodat ik mijn code ook een stuk kon opschonen. Echter, de grootste verandering was dat ik van de articles met de content allemaal een kubus heb gemaakt die rond draait met de content. Dit was een heel erg leuk idee van Sanne die erg hielp om de content A, wat makkelijker kwa ruimte te verdelen, en B op een leuke manier weer te geven, maar de uitvoering was toch iets lastiger, voornamelijk het dan ook nog eens responsive maken was extreem lastig en heb ik meerdere uren met Nils aan gezeten. 

De basis van de code en uitleg heb ik van Lorenzo gekregen, daarna heb ik zelf de code zo geschreven zodat ik alle vlakken kon zien, en de animatie toegevoegd, dat werkte allemaal nog behoorlijk soepeltjes. Toen heeft Sanne me geholpen met de hoogtet bepalen en zorgen dat deze op zo'n manier kon schalen dat het responsive kon zijn. Daarna, toen ik bezig begon met afstand tussen de blokken bepalen, ging het wat mis. Hierna heb ik Nils er dus bij geroepen en hebben we meerdere malen gekeken naar waarom de code niet helemaal normaal leek te gedragen. Een gedeelte hiervan lag aan de manier waarop Lorenzo zijn code in elkaar had gezet, wat ervoor zorgde dat de kubus uit het "scherm niveau" wordt geduwd, wat ervoor zorgt dat er best veel distortion is, wat vervelend in de weg kwam te zitten bij het positioneren. 

Daarbij heb ik de container queries verplaatst van het article, naar de popover met de button in het article. Ook heb ik in het algemeen extra content toegevoegd en de footer met een `detail` element erbij gedaan die animeert op in en uit klappen. 

Nesting van CSS
<img width="1470" alt="Screenshot 2025-03-17 at 11 39 42" src="https://github.com/user-attachments/assets/7b571b1c-10b7-4e85-963b-569dd3ac3782" />
<img width="1470" alt="Screenshot 2025-03-17 at 11 39 24" src="https://github.com/user-attachments/assets/7ca1a09e-80a2-4236-a207-148af1d8533e" />

Experiment om 3D blokken te maken en deze te roteren met de content
<img width="1470" alt="Screenshot 2025-03-18 at 11 55 20" src="https://github.com/user-attachments/assets/74087256-fd1b-437f-a0d2-edb142d88a84" />


# Bronnen
## Inception
* https://inception.fandom.com/wiki/City_(dream) 
* https://nl.wikipedia.org/wiki/Inception
* https://inception.fandom.com/wiki/Inception_Wiki
* https://screenrant.com/inception-movie-levels-dream-layers-how-many-explained/

## Code
### CSS Motion Path
* https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_motion_path 
* https://developer.mozilla.org/en-US/docs/Web/CSS/offset-distance
* https://developer.mozilla.org/en-US/docs/Web/CSS/offset-position

### Stroke 
* https://developer.mozilla.org/en-US/docs/Web/CSS/stroke 
* https://developer.mozilla.org/en-US/docs/Web/CSS/stroke-dasharray
* https://developer.mozilla.org/en-US/docs/Web/CSS/stroke-dashoffset
* https://developer.mozilla.org/en-US/docs/Web/CSS/stroke-linecap
* https://developer.mozilla.org/en-US/docs/Web/CSS/stroke-width

### Custom properties
* https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_cascading_variables/Using_CSS_custom_properties 
* https://developer.mozilla.org/en-US/docs/Web/CSS/--*
* https://codepen.io/shooft/pen/ZEMWOPj

### Helping tools
* https://wakamaifondue.com/beta/
