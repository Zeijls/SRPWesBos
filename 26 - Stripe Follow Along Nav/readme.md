Je kunt de dropdowns makkelijk laten weergeven met CSS. De reden dat het in deze les met Javascript wordt gedaan is omdat er wordt gekeken hoe breed de inhoud van iedere dropdown is, en de background daarop wordt aangepast. Dit doe je door; 

 const coords = {
      height: dropdownCoords.height,
      width: dropdownCoords.width,
	  top: dropdownCoords.top,
      left: dropdownCoords.left,
    };

    background.style.setProperty('width', `${coords.width}px`);
    background.style.setProperty('height', `${coords.height}px`);
    background.style.setProperty('transform', `translate(${coords.left}px, ${coords.top}px)`);
  }

In principe werkt het nu naar behoren alleen zodra er een h2 element of iets dergelijks wordt toegevoegd, klopt de hoogte niet meer helemaal. Dit maak je door de volgende regel toe te voegen;

 top: dropdownCoords.top - navCoords.top,
 left: dropdownCoords.left - navCoords.left,
 
 De content flipt nu als je er heel snel overheen gaat, dit komt doordat het element al wordt aangemaakt voordat je erover heen hovert. Dit maak je door deze regel in een if statement te zetten; 
 
 setTimeout(() => this.classList.contains('trigger-enter') && this.classList.add('trigger-enter-active'), 150);
    background.classList.add('open');
	
