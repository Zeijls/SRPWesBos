# 25 - Event Capture, Propagation, Bubbling and Onces

Als je klikt op div three klik je indirect op alle elementne waar deze div in is genest. Hierdoor triggert het ook een click op al deze elementen. 

Hoe het werkt in moderne browsers;
De browser kijkt vanaf het HTML element waar div three in is genest van buiten naar binnen, dus one > two > three. En begint daarna van three naar one te "bubble up" wat betekent dat hij de events triggert in de volgorde three > two > one. 

zodra je "capture=true" toevoegt betekent dit dat hij liever van buiten naar binnen de code runt dan van binnen naar buiten. Dus; one > two > three. (by default it is false)

e.stopPropagation(); = stop bubble up the event

New property; once

capture; false,
once: true

hierdoor luisterd het eenmalig naar een click, en "unbined itself" zodat er geen toekomstige clicks meer zijn. (Hierdoor kun je een keer klikken en daarna werkt het niet meer tot dat je de pagina herlaad)

[Opdracht 25](https://zeijls.github.io/SRPWesBos/25/index-START.html) <br>

[Terug naar het overzicht](https://zeijls.github.io/SRPWesBos/)


