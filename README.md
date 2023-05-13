<h1 align="center">JavaScript Lesson #2</h1>
<h2 align="center">Table of contents</h2>

1. SCOPE
   + GLOBAL SCOPE
   ```javascript
   const name = "Jonas";
   var name = "John";
   let name = "Jennyfer";
   ```
   + FUNCTION SCOPE
   ```javascript
   function age(x){
       let yearOfBirth = 1887;
       return 2023 - 1887
   }
   ```
   + BLOCK SCOPE
   ```javascript
   if(n > a){
       console.log("true")
   }
   for(let i=1;i<=x;i++){
       sum += i;
   }
   ```
   + MODULE SCOPE
2. HOISTING
    + VAR
    ```javascript
    a = 2;
    var a;
    console.log(a);
    ``` 
    + FUNCTION DECLARATION
    ```javascript
    foo():

    function foo(){
        console.log(a) //undefined

        var a=2;
    }
    ``` 

<br><br><br>
<h2 align="center">TEMPORAL DEAD ZONE</h2>

<h2 align='center'>LET & CONST</h2>

```javascript
const name = "John";

if(name === "John"){
    console.log(`John is a best`, ${job})
    const age = 2023 - 2007;
    console.log(age)
    const job = "Cooker";
    console.log(x)
}
```
<br><br><br>

1. RECURSION
```javascript
    function recurse(){
        if(condition){
            recurse();
        }
        else{
            // stop calling recurse 
        }
    }
```
2. CLOSURE
```javascript
const secureBooking = function () {
    let passengerCount = 0;

    return function () {
        passengerCount++;
        console.log(`${passengerCount} passengers`)
    };
};

const booker = secureBooking();
booker();
booker();
```
