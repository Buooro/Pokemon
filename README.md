
var opcion =  prompt("Elige un pokemon \n 0: Pikachu \n 1: Charmander \n 2: bulbasaur",0);
var tipo = ["Electrico","Fuego","Tierra"];


function Pokemon(n,v,a)
{
	var gritos = ["Pikachu","Charmander","Bulbasaur"];
	this.grito = gritos[opcion]
	this.nombre = n;
	this.vida = v;
	this.ataque = a;

	this.gritar = function(){
alert(this.grito);
	}
}



function eleccion(){

if (opcion == 0 ){
	gritar();
	var pika = new Pokemon("Pikachu",93,90);
nombrePokemon.textContent = "Nombre del Pokemon: " + pika.nombre +  "Vida del Pokemon: " + pika.vida + "Ataque: "+ pika.ataque + "Tipo: "+ tipo[opcion];
document.write("<img src= https://s-media-cache-ak0.pinimg.com/originals/aa/55/7c/aa557c9bef8b8fab87c5e9f63cca7efd.png width=\"100\" height=\"100\" /> </img>");
document.write("<audio src = http://vignette2.wikia.nocookie.net/es.pokemon/images/1/19/Grito_de_Pikachu.ogg/revision/latest?cb=20140805103956 autoplay controls</audio>");
}
else if (opcion ==1){
		
var charm = new Pokemon("Charmander",100,50);
gritar();
nombrePokemon.textContent = "Nombre del Pokemon: " + charm.nombre +  "Vida del Pokemon: " + charm.vida  + "Ataque: "+ charm.ataque + "Tipo: "+ tipo[opcion];
document.write("<img src= http://img2.wikia.nocookie.net/__cb20140603214909/pokemon/images/4/41/004Charmander_OS_anime_2.png width=\"100\" height=\"100\" /> </img>");
document.write("<audio src = http://vignette4.wikia.nocookie.net/es.pokemon/images/4/47/Grito_de_Charmander.ogg/revision/latest?cb=20140731190207 autoplay controls</audio>");

	}
	else if (opcion==2){
var Bul = new Pokemon("Bulbasaur",13,30);
gritar();
nombrePokemon.textContent = "Nombre del Pokemon: " + Bul.nombre + "Vida del Pokemon: " + Bul.vida + "Ataque: "+ Bul.ataque + "Tipo: " + tipo[opcion];
document.write("<img src= http://images2.wikia.nocookie.net/__cb20111221113429/bulbasaurfanon/images/4/43/Bulbasaur.png width=\"100\" height=\"100\" /> </img>");
document.write("<audio src = http://vignette3.wikia.nocookie.net/es.pokemon/images/3/3a/Grito_de_Bulbasaur.ogg/revision/latest?cb=20140731185900 autoplay controls</audio>");

	}
else{
		alert("El pokemon no existe");
	}
	};




