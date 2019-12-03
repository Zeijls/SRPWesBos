# 16 - Mouse Move Shadow

Het belangrijkste wat ik in deze les heb geleerd is hoe je omgaat met offsetX en offsetY om uit te zoeken waar je cursos is. 

Zodra er elementen hierin zijn genest kun je dit oplossen door een kleine rekensom zoals onderstaande;

if (this !== e.target) {
				x = x + e.target.offsetLeft;
				y = y + e.target.offsetTop;
			}
			
Verder is het begrip "this" in deze les gebruikt. Het linkt in dit verhaal naar de div hero. 

${…} 
Door het $-teken identificeert hij een object hetzelfde als een naam zou doen.

[Opdracht 16](https://zeijls.github.io/SRPWesBos/16/index-START.html/) <br>

[Terug naar het overzicht](https://zeijls.github.io/SRPWesBos/)