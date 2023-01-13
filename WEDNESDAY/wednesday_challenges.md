# WEDNESDAY CHALLENGES WEEK 7

## Count strings in an object

![image](https://user-images.githubusercontent.com/117783981/212240269-3ad110d9-ddc1-4949-bece-79eedbc1b7f4.png)



function strCount(obj){
  let count = 0; // Initialize counter
  for (key in obj){ // The "key" is the argument inside the object
     console.log(key + " : " + obj[key] + " : " + typeof obj [key]);
    if (typeof obj[key] == 'string') count++; // Typeof allows us to identify the type of object
    if (typeof obj[key] == 'object') count = count + strCount(obj[key]); // Recursion, the function calls itself to count inside object types
    
  }
  
  console.log(count);
  return count
}


## Extending JavaScript Objects: Get First & Last Array Element

![image](https://user-images.githubusercontent.com/117783981/212242255-5bd6b01e-b8bd-486d-9a63-084aab5c64d7.png)


/*
La propieda prototype nos permite agregar objetos a un array
o nuevas variables a los objetos.

Se agrega el metodo first y se crea una funcion que retorna el primer
ojeto del array. Se usa this[] porque uno se esta refiriendo al mismo objeto.

Para el ultimo elemento del array se utiliza this.length - 1 porque los arrays
empiezan desde cero
*/

Array.prototype.first = function() {
  return this[0];
};

Array.prototype.last = function() {
  return this[this.length-1];
};


## Object Oriented Piracy

![image](https://user-images.githubusercontent.com/117783981/212246684-c96faf6f-5620-4a4c-ad58-94d4c7004915.png)


![image](https://user-images.githubusercontent.com/117783981/212246660-aad89dcd-4300-4752-8a0f-061409b8ced3.png)



/*
the keyword "this" refers in this case to the object ship
isWorthIt is a new property/method of the ship object
We assign the isWothIt method a function and this function
makes the evaluation a return a true/false value
*/

function Ship(draft,crew) {
 this.draft = draft;
 this.crew = crew;
  this.isWorthIt = function() {
    return (this.draft - this.crew * 1.5) > 20;
}
  }
