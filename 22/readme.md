# 22 - Follow Along Link Highlighter

Om uit te zoeken waar op de pagina de linkjes zich bevinden en welke hoogte en breedte zij hebben kun je de volgende regels gebruiken. Hierdoor komt alle info in je console te staan.

	  function highlightLink(){
		  const linkCoords = this.getBoundingClientRect();
		  console.log(linkCoords);
		  
		  
De hover werkt nu goed, alleen zodra je naar onder scrollt klopt de plaatsing niet meer. Dit heeft te maken met de X en Y van de pagina. Om dit op te lossen gebruik je de volgende regels.

const coords = {
      width: linkCoords.width,
      height: linkCoords.height,
      top: linkCoords.top + window.scrollY,
      left: linkCoords.left + window.scrollX
    };
	
	
[Opdracht 22](https://zeijls.github.io/SRPWesBos/22/index-START.html) <br>

[Terug naar het overzicht](https://zeijls.github.io/SRPWesBos/)