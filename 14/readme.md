# 14 - Javascript References VS Copying

Als je een kopie van een array update, zal hij dit altijd terughalen uit de bron. Als in het voorbeeld;

const players = ['Wes', 'Sarah', 'Ryan', 'Poppy'];

const team = players;

console.log(players, team);

team[3] = 'Lux';

Als je nu in de console het team aanroept is het antwoord;
['Wes', 'Sarah', 'Ryan', 'Lux']

Maar als je nu in de console de players aanroept krijg je hetzelfde antwoord.

Om dit op te lossen kun je een kopie maken van de array, dit doe je door;

const team2 = players.slice();
Nu zal het 4e teamlid in het team wel worden aangepast, maar bij de players niet.

Of door een nieuwe array te amken en de oude te "concat"
const team3 =[].concat(players);
Hierdoor worden alle items uit de array in de lege array geplaatst. 

Of gebruik de nieuwe ES6 spread
De spread neemt alle items uit de array, en plaatst ze 1 voor 1 in de nieuwe container array.

const team4 = [...players];
team4[3] = 'heee haawww';
console.log(team4);

const team5 = Array.from(players)\

Werkt hetzelfde voor objects

{...person} Werkt precies hetzelfde als de spread van bovenstaand array, alleen spread je hier in een object

Op dit moment pakt hij alleen de eerste laag, zodra je dieper in het element wilt moet je de lagen clonen. Dit kan, alleen vraag je wel eerst af of dit echt nodig is, of dat er misschien een betere en duidelijkere manier is. 

Dit doe je door;

const dev = Object.assign({}, wes);
const dev2 = JSON.parse(JSON.stringify(wes));

Nu wordt hij niet aangepast doordat jason.stringify er een string van maakt, in plaats van een object. En door de JSON.parse wordt hij weer terug veranderd naar een object. 

In deze les is het object aan bod gekomen. Hier is niet dieper op in gegaan, maar vooral besproken hoe je deze kunt aanpassen naar een array.

Begrippen
Functions
-	Scope
-	Event Loop
-	Asynchroon
-	Hoisting
-	Closure

Objecten
-	Object literal/constructor
-	Context (this)

[Opdracht 14](https://zeijls.github.io/SRPWesBos/14/index-START.html) <br>

[Terug naar het overzicht](https://zeijls.github.io/SRPWesBos/)
