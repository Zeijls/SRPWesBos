Om een ancherpoint te maken vanaf waar de gebruiker de muis ingedrukt houdt en naar links of rechts te slepen gebruik je de volgende regels in de mousedown;

startX = e.pageX - slider.offsetLeft;

e.preventDefault();
Dit zorgt ervoor dat alles waarvan de browser denkt dat je dit probeert te selecteren, zoals tekst of iets dergelijks, dit zorgt ervoor dat dit wordt gedeselecteerd.

Uitzoeken waar de cursos is als er iets is bewogen. We weten al waar de cursor is als er is geklikt, maar nu moeten we nog weten waar hij is zodra er is bewogen.

const x = e.pageX - slider.offsetLeft;