# 15 - Local Storage

addItems.addEventListener('submit', );

In deze regel gebruiken we submit omdat dit naar alle vormen luistert, en niet alleen naar het klikken op de button. (Dus enter klikken enzovoort...)
Hierdoor zorg je dat je veilig zit en alle manieren hebt gedekt. 

e.preventDefault();
Zorgt ervoor dat de pagina stopt met zichzelf te herladen. Dit komt doordat in de "default" de data stuurt zichzelf naar een externe bron, zodoende prevent de default zodat dat niet gebeurd.

Om het imput veld weer te legen
this is een form element, en form elements hebben een method genaamd reset.  

Iedere keer als er op de button wordt geklikt, wordt de functie populateList aangeroepen. In deze functie wordt een label aangemaakt met de ingevoerde tekst. 

Local Storage

localStorage.setItem('items', JSON.stringify(items));

JSON.stringify = array > object
JSON.parse = object > array

wat er nu gebeurd in de file; zodra je een item toevoegd wordt deze opgeslagen in localStorage, en zodra een pagina wordt herladen wordt er gecontrolleerd of er iets is opgeslagen in LocalStorage, maar zo niet valt hij terug op de lege array. 

De begrippen zijn in deze lessen niet naar voren gekomen

[Opdracht 15](https://zeijls.github.io/SRPWesBos/15/index-START.html/) <br>

[Terug naar het overzicht](https://zeijls.github.io/SRPWesBos/)