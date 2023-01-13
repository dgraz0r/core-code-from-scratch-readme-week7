# WEDNESDAY CHALLENGES WEEK 7

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
