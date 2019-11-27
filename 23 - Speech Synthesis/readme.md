function setVoice(){
			msg.voice = voices.find(voice => voice.name === this.value)
			
Door deze functie zal een loop alle stemmen in de array controleren, en vind hij het atribuut waarbij de naam hetzelfde is als de optie die op dit moment is geselecteerd. 