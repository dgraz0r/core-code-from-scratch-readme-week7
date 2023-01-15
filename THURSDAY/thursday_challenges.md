# THURSDAY CHALLENGES


## Convert a String to a Number!

![image](https://user-images.githubusercontent.com/117783981/212460560-d4f78ad0-abf1-4d12-8204-bb1f0c64b605.png)


const stringToNumber = function(str){
  // By using the type of object we want in the return statement and passing the string as argument the string is converted into a number
  return Number(str);
}


## Convert number to reversed array of digits

![image](https://user-images.githubusercontent.com/117783981/212490364-f7ceda43-ded5-4a2f-be6a-e58d74f6ab5d.png)


/*
El argumento n es de tipo numerico por lo cual lo convertimos a string con
String(n), luego utilizamos la function split('') para convertir cada palabra
del string a un elemento de un array, si no se colocan '' en la funcion split
entonces todo el string sera un solo elemento del array.

Para que el array este de forma inversa se usa la funcion reverse y para que los
elementos del array sean numeros usamos la funcion map(Number) con el argumento
Number para que reciba el array en forma de string y lo devuelva en forma numerica

*/

function digitize(n) {
  return String(n).split('').reverse().map(Number)
}

## Truthy and Falsy

![image](https://user-images.githubusercontent.com/117783981/212524964-6bf40f26-6b85-4c00-ad87-b53006ab550c.png)


/*
Truthy and falsy values are defined by javascript, always check documentation.
*/

const truthy = [-42, true, {}, "false", []];
const falsy = [false, 0, "", null, NaN];


