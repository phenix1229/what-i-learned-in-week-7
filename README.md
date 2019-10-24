# what-i-learned-in-week-7
## `for` loops

An (preferred?) alternative to `while` loops.

*Example*
```
const numbers = [1,3,5,9,10];

for (let i = 0; i < numbers.length; i++){
    console.log(numbers[i] * 3);
}

results - 3, 9, 15, 27, 30
```

---

## String building

Since you cannot change characters in a string (mutate), you must build a new string based on the string you want to change.

*Example*
```
const string1 = '$100 < $1 right?';
let newStr = '';

function makeGreater(){
    for (let i = 0; i< string1.length; i++){
        if (string1[i] === '<'){
            newStr = newStr + '>';
        } else {
            newStr = newStr + string1[i];
        }
    }
    return newStr;
}
```
String theory exercise: https://github.com/ci-wdi-900/string-theory

---

## Map

A map is a one to one transformation of values. In other words, each value is 'mapped' to another value.

*Example*
```
function oddOrEven(arr) {
  for (let i = 0; i < arr.length; i++){
    if (arr[i] % 2 === 0){
      arr[i] = 'even';
    } else {
      arr[i] = 'odd';
    }
  }
}
```
Mapmaker exercise: https://github.com/ci-wdi-900/mapmaker-mapmaker

---

## Troubleshooting someone else' code

CBBT exercise: https://github.com/ci-wdi-900/cripples-bastards-and-broken-things 

P I T A 

---

## Miscellaneous
### Slice

`str.slice(start, stop)` - gives items from a string or array beginning with the starting index (if given, 0 if not) and ending one index before the stop index (if given, last index if not). It can start from the end of the string or array if the starting index is a negative number.

*ps: `slice` don't `splice`*