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