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

# Bronnen
## Inception
* https://inception.fandom.com/wiki/City_(dream) 
* https://nl.wikipedia.org/wiki/Inception
* https://inception.fandom.com/wiki/Inception_Wiki

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