# 10 - Hold Shift and Check Checkboxes

IN between 

Deze functie gaat alle elementen van het DOM element af om ze een voor een te checken.

inBetween = !inBetween 
gebruik je omdat inBetween true en false moet zijn om het zelfde moment.

if (checkbox === this || checkbox === lastChecked) {inBetween = !inBetween;)

checkbox === this ~ Is de checkbox die wordt aangeklikt

checkbox === lastChecked ~ Geld voor de laatste checked box 

if (inBetween) {checkbox.checked = true; }
Door deze regel worden alle boxen hiertussen gechecked

In deze les heb ik kennis gemaakt met inBetween. Ik heb verder geen van de onderstaande begrippen geleerd;

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

[Opdracht 10](https://zeijls.github.io/SRPWesBos/10/index-START.html/) <br>

[Terug naar het overzicht](https://zeijls.github.io/SRPWesBos/)