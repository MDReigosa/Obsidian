
pwd
ls
mkdir
mkdir -v
cd
cd ../
touch
rm
-- help
code
git status
git add
git init
git commit -m ".." guarda
git log
git remote add origin
git branch -M main
git push -u origin main envia a base datos
rm remove





JAVA
strings
numeros
booleanos
undefined
null
console.log
function sumaTres(x) {

    console.log(x+3);

}
return

Camelcase: holaMundo
Pascalcase: HolaMundo
snake_case: hola_mundo


Condiciones
function viajar(destino) {

    if (destino === "brasil") {

        console.log("gire a la izq");

       } else if (destino ==="argentina") {

        console.log("gire a la derecha");

       } else {

        console.log("te perdiste");

       }

}

math.pow: potenciar numero
math.round: redondea (si <0.49 o >0.5)
math.floor : redondeará el número decimal al entero de menor valor
Math.ceil: redondeará el número decimal al entero de mayor valor
math.max
math.min
math.random(): random decimal
npm test


&& and
|| or
! not  !(5 < 2) true

//AND
function mayorYMenorYPar(num) {
	if( num > 5 && num < 10  && num  % 2 === 0 ) console.log(true);
	else console.log(false);
};
mayorYMenorYPar(7);
mayorYMenorYPar(8); 

// OR
function operadorOr(str) {
   if (str === 'Henry' || str.length < 2) console.log(true);
   else console.log(false);
}
operadorOr('Henry');
operadorOr('Javascript');
operadorOr('H');

// NOT
function negacion(permiso) {
   if (permiso) console.log('Tiene permiso');
}
negacion(true);
negacion(false);

FOR: sabemos con anticipacion la cantidad de pasos

for(var i=0 ; i<5 ; i++){

   hola = hola + 1;

   console.log("variable de iteracion: ", i);

}

console.log("variable de suma:  ", hola)

while: no sabemos con anticipacion

while (hola < 15){

   hola = hola + 1;

   console.log(hola)

}


let result = '';
let i = 0;

do {
  i = i + 1;
  result = result + i;
} while (i < 5);

console.log(result);


continue
do..  while
case
default

switch
```
var Animal = 'Jirafa';
switch (Animal) {
  case 'Vaca':
  case 'Jirafa':
  case 'Perro':
  case 'Cerdo':
    console.log('Este animal subirá al Arca de Noé.');
    break;
  case 'Dinosaurio':
  default:
    console.log('Este animal no lo hará.');
}
```
```
switch (expr) {
  case 'Naranjas':
    console.log('El kilogramo de naranjas cuesta $0.59.');
    break;
  case 'Manzanas':
    console.log('El kilogramo de manzanas cuesta $0.32.');
    break;
  case 'Platanos':
    console.log('El kilogramo de platanos cuesta $0.48.');
    break;
  case 'Cerezas':
    console.log('El kilogramo de cerezas cuesta $3.00.');
    break;
  case 'Mangos':
  case 'Papayas':
    console.log('El kilogramo de mangos y papayas cuesta $2.79.');
    break;
  default:
    console.log('Lo lamentamos, por el momento no disponemos de ' + expr + '.');
}

console.log("¿Hay algo más que te quisiera consultar?");

ARRAY
var listadecompras = [];

listadecompras[3] = "tomate";

  

// console.log(listadecompras)

  

var elementosdecompra = listadecompras[3];

  

console.log(elementosdecompra);



var nombres = ['Matias', 'Maria', 'Diego', 'Rosa'].length;
console.log(nombres);


var colores =["amarillo", "rojo"];

colores.push("azul"); AGREGA AZUL AL FINAL

console.log(colores.length);
colores.unshift("verde"); DA VERDE EN PRIMERA POSICION

colores.pop() elimina ultimo
colores.shift() elimina primero



var numeros = [10, 10, 8 , 5];

var cumplecondicion = numeros.every((num) => {

    return num >5;

});

console.log(cumplecondicion);
DA TRUE O FALSE SI TODOS SON > 5

SEPARAR LETRAS

var palabra = "Henry";

var palabraseparada = palabra.split("");

  

console.log(palabraseparada);


ARREGLAR UNA PALABRA


var palabra = "Henri";

var palabraseparada = palabra.split("");

palabraseparada.pop();

palabraseparada.push("y")

var palabraarreglada = palabraseparada.join("");

console.log(palabraarreglada);



  
-   El método **forEach**() nos permite recorrer un arreglo, realizando alguna acción en para cada elemento.
           
    El método **map**() también nos permite recorrer un arreglo y realizar una acción por cada elemento. La diferencia es que este método devuelve un nuevo arreglo los elementos modificados.
var numeros = [1,2,3,4];

/*

numeros.forEach((num) => console.log(num));

numeros.forEach((num) => {

    if (num === 3); {

        console.log(num);

    }

});

*/

  

var numerosmasuno = numeros.map((num) => {

    return num + 2;

    });

    console.log(numerosmasuno);


function encontrarletrap(string) {

var letras = string.split("");

for(let i = 0; i <letras.length; i++) {

    if(letras[i] === "p") {

        console.log("si contiene a P");

    }

}

}

  

encontrarletrap("Javascript");

encontrarletrap("HEnry");