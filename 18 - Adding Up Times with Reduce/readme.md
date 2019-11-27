Voor deze oefening gaan we kijken hoe we deze tijdstippen uit het DOM model kunnen halen. Converteren naar nummers, daarna naar minuten en seconden. Uitzoeken hoeveel uren minuten en secondes dit in totaal zijn en uiteindelijk deze waardes console.log ' en.

Veranderen van een NodeList naar een nieuwe array;
Array.from()

Nodelist = een array van list items
door array.from veranderd in een array van strings

	const [mins, secs] = timeCode.split(':');
Door deze regel worden de minuten en secondes van elkaar gescheiden, alleen zitten ze nog steeds in dezelfde string. Hierdoor kun je hier niet mee gaan rekenen en moet je ze eerst omzetten. Dit doe je door;

.map(parseFloat) > hierdoor worden alle items in de string van elkaar los gemaakt. Hierdoor worden de items in de array daadwerkelijk nummers. 

om de minuten en secondes samen te voegen kun je een reduce gebruiken

als een map een array in en exporteert kan een reduce een array aannemen en exporteren in wat je wilt. 

Reduce = importeert een array en exporteerd de array in wat je maar wilt (string, nummer enz.) in dit geval een nummer

Math = 100 based
minutes = 60 based

% houdt bij hoeveel hele er over blijven die niet kunnen worden verdeeld. 
11/5 = 2.2 maar in javascript zou dit als uitkomt 2 geven en blijft er 1 hele over. 

Met % houd hij bij hoeveer er over blijft. 

Oftwel " hoeveel blijven er over als ze door hele zijn verdeeld. "