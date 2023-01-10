# MONDAY CHALLENGES

## String: substr()

function firstWord(s1) {
let blank = s1.indexOf(" ");
return s1.substr(0, blank);
}

let test = firstWord("see and stop")

## String: replace()

function normalize(s1) {
return s1.replace(/-/g, "/")
}

let test = normalize("20-05-2017") 

## Increment

let x = 3;
x++;
x = x * 2;
x--; // The answer is 7 

## Fahrenheit

function toFahrenheit(t) {
let F = 1.8 * t + 32;
return F;
}

let result = toFahrenheit(0)
