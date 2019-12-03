# 28 - Video Speed Controller

Om de interfase mee te laten bewegen met de click and drag gebruik je het volgende;

const speed = document.querySelector('speed');
	const bar = speed.querySelector('.speed-bar');
	const video = document.querySelector('.flex');
	
	speed.addEventListener('mousmove', function(e) { 
		const y = e.pageY = this.offsetTop;
		
		
Hij werkt nog niet volledig omdat hij geen uitkomst in procenten weergeeft. Dit doe je door het volgende

	const percent = y / this.offsetHeight;
		const min = 0.4;
		const max = 4;
		const height = Math.round(percent * 100) + "%";
		bar.style.height = height;
		
Nu moet het getal in de balk ook worden geupdate zodra er een mousemove is;

De playbackrate moet niet van 0 naar 100, maar van 0,4 naar 4. Om dit te laten werken moet er een klein beetje rekenen worden toegepast;

const playbackRate = percent * (max - min) + min;
		bar.style.height = height;
		bar.textContent = playbackRate.toFixed(2) + "x";
		video.playbackRate = playbackRate;

[Opdracht 28](https://zeijls.github.io/SRPWesBos/28/index-START.html/) <br>

[Terug naar het overzicht](https://zeijls.github.io/SRPWesBos/)