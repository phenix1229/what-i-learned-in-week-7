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

## String building

Since you cannot change characters in a string (mutate), you must build a new string based on the string you want to change.

*Example*
```
const string1 = '$100 < $1 right?';
let newStr = '';

function makeGreater{
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
