
# <span style="color:">missingskill-learning
![Image](https://github.com/nikhilgotpagar/METRepository/blob/main/a2ea924c-aeb5-45d2-9d87-3d192c50b515.jpg?raw=true)
# JavaScript




#
#
**Created By : Nikhil Gotpagar**
#
#
#

---

### <span style="color:Gray"> 1. History Of  JavaScript
### <span style="color:Gray"> 2. JavaScript Framework
### <span style="color:Gray"> 3. Control Structures
### <span style="color:Gray"> 4. Tech Debt
### <span style="color:Gray"> 5. DataTypes
### <span style="color:Gray"> 6. Copy By value & Copy By reference
### <span style="color:Gray"> 7. JavaScript functions.
### <span style="color:Gray"> 8. IIFE, Inline functions.
### <span style="color:Gray"> 9. Constructors & Prototypes.
### <span style="color:Gray"> 10. Array, Objects & String prototype methods.
### <span style="color:Gray"> 11. Built in functions & ES6.

---

#### <span style="color:Gray"> 1. History Of  JavaScript

In 1991 **linux** was launched and tech revolution started. Microsoft and Apple were big players of market. Netscape browser was the only way to use internet, Microsoft build Internet Explorer and provided it for free for users. Java was very strong backend language but it was missing frontend part. To complete that void Netscape programmer named **Brandan Eich developed a new programming language in just 10 days**.It was originally named Mocha.Later, the marketing team replaced the name with 'LiveScript'. Later due to licensing issue JavaScript name came into existence. Around 95 % websites were created using Javascript. JavaScript has no connectivity with Java programming language.

**MIT License :**
The MIT license gives users  permission to reuse code for any purpose, sometimes even if code is part of proprietary software. As long as users include the original copy of the MIT license in their distribution, they can make any changes or modifications to the code to suit their own needs.
Neither distributor nor the devloper is responsible for the damaged done by code system (If in case).
#
#
#
#
#
#

---
### <span style="color:Gray"> 2. JavaScript Framework
>JS frameworks are collections of JavaScript code libraries that provide developers with pre-written JS code.

**Some of the popular framework of JavaScript are :**
1. <span style="color:Red"> Angular JS
2. <span style="color:blue">React JS
3. <span style="color:aqua"> Vue JS
4. <span style="color:Green">Node JS
5. <span style="color:darksalmon">Ember JS
6. <span style="color:Navy"> Backbone JS
#
#
#
#
#
#
#
#
---
### <span style="color:Gray"> 3. Control Structures & Operators
**Control Structure:**
- If else : Often used
- for : abstrcations
- switch case : better way available in js
- while : normal use
- do while : normal use
#
**Operators:**
1. Arithmetic
2. Logical
3. Bitwise
4. Ternary
5. Relational
#
1. Arithmetic

| Operator | Use | 
|--- |--- |
| + | Addition |
| - | Subtraction |
| * | Multiplication |
| / | Division |
| % | Modulus |
| ++ | Increment |
| -- | Decrement |

2. Logical

| Operator | Use | 
|--- |--- |
| && | AND |  
| ! | Not |

| Logical AND | . |
|--- |--- |
|true && false | false |
|false && false | false |
|false && true | false |
|true && true | true |

#
 Logical OR | . |
|--- |--- |
|false && true | true |
|true && false | true |
|true && true | true |
|false && false | false |


3. Bitwise

| Operator | Use |
| --- | --- |
| &| Bitwise AND|
| ^ | Bitwise XOR |
|~| Bitwise NOT |
| << | Bitwise Leftshift |
| >> | Bitwise RightShift |
| >>> |Bitwise Rightshift with zero |
#
#
---
### <span style="color:Gray"> 4. Tech Debt

+ ( cocat & addition ) : a + a = aa
- === : Equality check
- Type of Null : **Object**.
#
#
#
#
#

---
### <span style="color:Gray"> 5. DataTypes
> Javascript is a dynamic type language 

Types :
1. Primitive Datatypes : ( Copy By value)

| Datatype | Use | 
|--- |--- |
| string | Represents a character |
| Number | Represents numeric values |
| Boolean | Represents True or False |
| Undefined | Represents Undefined value |
| Null | Represents Null |

2. Non - primitive Datatype : (Copy By Reference)

| Datatype | Use | 
|--- |--- |
| object | Represents instance through which we can access members |
| Array | Represents group of values |
| RegExp | Represents regular expression |

**Practicals :**
```
>a = null
>null
>typeof a
>object 
```
#
```
>a = {}
>{}
>typeof a
>"object"
```
#
| var | let | const |
|--- |--- | --- |
|can be redecalred |As per ES6 standard let cant be redeclared| As per ES6 standard can not be redeclared|
|can be reinitialized |can be reinitialized|cant be reinitialized but NP values can be updated|
|functional scope|lexical scope|lexical scop|
|ES5 | ES6|ES6|
|hoisted| Doesnt get hoisted|Doesnt get hoisted|

```
>var num = 10;
>undefined
>var val = "call";
>undefined
>num + val
>"10call"
```
```
var num = 10;
undefined
var num1 = 20;
undefined
num + num1
30
```
```
var cost= 100;
undefined
var tax = 0.18;
undefined
var value = cost * tax
undefined
value
18
```

```
>var cost= "100";
>undefined
>var tax = 0.18;
>undefined
>var value = cost * tax
>undefined
>value
>10018
```

```
>cost + +tax
>100.18
>+cost + +tax
>100.18
>(+cost) + (+tax)
>100.18
```
```
var arr =[];
undefined
typeof arr
"object"
```
```
var arr = [2]
undefined
var arr2 =[2,3,null]
undefined
console.log(arr.length);
1
arr +arr2
"22,3,"
```
```
var arr =[2, 3, 3, null,true, [], {}]
undefined
arr [4]= 67;
67
console.log(arr);
VM2358:1 (7) [2, 3, 3, null, 67, Array(0), {…}]
```
```
var hello = { name : "nikhil", location : "mumbai"};
undefined
hello
{name: "nikhil", location: "mumbai"}
location: "mumbai"name: "nikhil"
__proto__: Object

hello.exp=12;
12
hello.role= "manager";
"manager"
hello
{name: "nikhil", location: "mumbai", exp: 12, role: "manager"}
```
**Lexical scope:**
Any scope inside a functional block.


>In a functional scope where you defined a variable it always gets hoisted at the top

```
function hello(){ //functional scope
    if (a){
        //lexical scope
    }else{
        //lexical scope
    }

}

if variable is ES6 iwt will check in lexical scope first, then parent lexical scope, function scope,parents scope.....
```

![Image](https://github.com/nikhilgotpagar/METRepository/blob/main/hosit.jpeg?raw=true)
#
#
#
---

### <span style="color:Gray"> 6. Copy By value & Copy By reference

- Copy by value : Xerox (if someone makes update then its updted the copy not the orginal assignment )
- Copy by reference : Google Docs. (passing reference to the other person. It doesnt matter how many reference you give your updating the same docs)
Banking acct (Accounts with multiple cards for same account . cards holding reference to the money use any card to deduct both cards will get updated for same account.)

Copy By Value code :
```
var stack = {
    node :1,
    php : 1,
    go :1,
    es : [5,6,7,8,9,10]
}
console.log("1",stack);
 
var tech = stack; // type of stack is object, objects are non primitive or cbr
tech.go=10;
console.log("3",stack);
var cloud ={

}

Output:
PS C:\Users\ADMIN\Desktop\JScode> node cpv.js
1 { node: 1, php: 1, go: 1, es: [ 5, 6, 7, 8, 9, 10 ] }
3 { node: 1, php: 1, go: 10, es: [ 5, 6, 7, 8, 9, 10 ] }
```

Call By Reference code :
```
var stack = {
    node :1,
    php : 1,
    go :1,
    es : [5,6,7,8,9,10] // np
}
var cloud ={
    aws :1,
    google : 1,
    do: 1
}

 
var tech = stack; // type of stack is object, objects are non primitive or pbr
var provider = cloud ; // np value 
cloud.js= stack.es;
stack.node={
    aws : cloud.aws
}
cloud.js[3]= "Arrow";
console.log("3",stack,provider);

Output:
PS C:\Users\ADMIN\Desktop\JScode> node cpr.js
Debugger attached.
3 { node: { aws: 1 }, php: 1, go: 1, es: [ 5, 6, 7, 'Arrow', 9, 10 ] } { aws: 1, google: 1, do: 1, js: [ 5, 6, 7, 'Arrow', 9, 10 ] }
```
---
#
### <span style="color:Gray"> 7. JavaScript Functions.

> JavaScript function is a block of code designed to perform a particular task.
It is executed when you invoked it.

**Properties of function :**
1. Hoisting.
2. Scope(local /global)
3. Overrride
4. Act as a container

**Function Behaviour :**
1. Normal declaration using function name.
2. Hoisting.
3. Override function.
4. Container (Object).
5. Scope local and global.
6. First class citizen
    a. function can be assigned to a variable.
    b. function can be returned from another function.
7. FRN (function returns a function).
8. Declaration and assignment.


```
function a () {}
undefined
a
ƒ a () {}
a.prototype
{constructor: ƒ}
constructor: ƒ a()
__proto__: Object
```



Syntax :
```
function name (parameter 1, parameter2){
    //code to be executed ;
}
```
Example 1 :
```
function fn_name(){
    console.log(20);
}

function main(){
    function output(){
        console.log("from inside");
        fn_name();

        function fn_name(){
            console.log("200");
        }
    }
    console.log("from outside");
    fn_name();
    output();
}

main();

Output:
PS C:\Users\ADMIN\Desktop\JScode> node fn.js

from outside
20
from inside
200
```
Example 2 :
```
var sports = "chess";
var sports2 = "kabaddi";

function printsport(abc){
    console.log("sports",abc);
    function demand(){
        console.log("demand=",abc);
    }
    demand();
}
printsport(sports);
printsport(sports2);

console.log("outside sport",sports);
console.log("outside sport",sports2);

Output :
PS C:\Users\ADMIN\Desktop\JScode> node fn.js

sports chess
demand= chess        
sports kabaddi       
demand= kabaddi      
outside sport chess  
outside sport kabaddi
```
Example 4:
```
function Ticket (counter){
    console.log("counter",counter);
   
    var irctc = function (book){
        console.log("book",book);

    }
    return irctc();

}
Ticket();

Output :
counter undefined
book undefined
```

**Function Declaration :**
>You actually defined a function with a name (hosited).

>let and const dont get hosited. (Initialization = Error).

**Function Assignment :**
>You create anonymouse function and you assgined variable to it.You can assign it to multiple variables.

Example 4 : (Cascading)
```
var sport = function (){
    var cricket = function(player){
    var ipl = function(team){
    
        return team;
    }
    return ipl;

    }
    return cricket;

}
    var cricket = sport();
    var result = cricket("sachin");
    var final = result("MI");
    console.log(final);

    var res=sport()("sachin")("delhi");
    console.log(res);

    Output :
    C:\Users\ADMIN\Desktop\JScode>node cas.js
MI
delhi
```


>IPL function can only be called after the sport function is called.

---

### <span style="color:Gray"> 8. IIFE, Inline Functions.
**IIFE :** Immediately invoked function expression.(self executing function expression).
Can only run once.
>Private method implementation (Like private methods in Java)

```
Syntax:
(function(){

})();
```


```
(function(){
    console.log("Initializing...");
})()

Output :
C:\Program Files\nodejs\node.exe .\fn.js
Initializing...
```
```
var outside =(function(userid){
    console.log.apply("initialization...");
    let counter = userid;

    function hello(value){
        counter = counter + value ;
        console.log("printing hello",value, counter);
    }
    return (hello)
})(100);

console.log(typeof outside, outside);
outside(10);
outside(20);
outside(30);
outside(40);

Output :C:\Program Files\nodejs\node.exe .\fn.js
function ƒ hello(value){
        counter = counter + value ;
        console.log("printing hello",value, counter);
    }
printing hello 10 110
printing hello 20 130
printing hello 30 160
printing hello 40 200
```

---
### <span style="color:Gray"> 9. Constructors & Prototypes.
In JavaScript, whenever a function is created the prototype property is added to that function automatically. It mimics the Object oriented concept in java.
By using prototype property we can attach a method to any object/function constructor. 
Methods are the part of a class. functions are Independent.
Example : 
```
function person(name, exp){
    this.name = name;
    this.exp = exp;
}

person.prototype.getName = function(){
    return this.name //This keyword refers to an object
}
var Nikhil = new person("nikhil",15);
var Nick = new person("nick", 10);

console.log(Nikhil);

Output :
C:\Program Files\nodejs\node.exe .\fn.js
person {name: 'nikhil', exp: 15}

```
---
### <span style="color:Gray"> 10. Array, Objects & String prototype methods.

In javaScript array is nothing but Indexed based object.

**Push & Pop :**
Push : used to add element into array.
Pop : used to remove element from array.
Unshift : It add elements at the beginning of the array. //rarely used
Shift : shift removes value from the beginning of the array. //rarely used 
Array push and pop operates at the end of the array. 

Example :
```
var names = ("josh","nick","ethan","john","penny")

names pop()
names pop()
names pop()

console.log(names);

var names = ("josh","nick","ethan","john","penny")

names push("jack","jill");

console.log(names);

var names = ("josh","nick","ethan","john","penny")

names unshift("Carl");

console.log(names);

var names = ("josh","nick","ethan","john","penny")

names shift("Ben");

console.log(names);
```

**Concat :** Concat method is used to merge two arrays.
Example

```
var names = ("josh","nick","ethan","john","penny")
var names2 = ("jack","jill");

var new_array = names.concat(names2);
console.log.(names,new_array);
```
**Map & filter :**

```
filter_arr = names.filtre(function(item)){
    return !!item;
}

filter_arr2 = names.filtre(function(item)){
    return !!(typeof item == "boolean");
}
console.log(name2,filter_arr2);
```

**indexof :**

```
if(name2.indexof("Nikhil) !== -1) {
    console.log("Items found);
}else{
    console.log ("Item is not present in the array");
}
```
**String :**
1. to.LowerCase : convert string into lower case character.
```
var text = ("My name is Nikhil");
console.log(text.toLowerCase());

Output:
C:\Program Files\nodejs\node.exe .\fn.js
my name is nikhil
```
2. to.upperCase : convert string into upper case character.

```
var text = ("My name is Nikhil");
console.log(text.toUpperCase());

Output:
C:\Program Files\nodejs\node.exe .\fn.js
MY NAME IS NIKHIL
```

3. split : it will split the value.
```

var text = ("My name is Nikhil");
console.log(text.split(" "));

Output:
C:\Program Files\nodejs\node.exe .\nik.js
(4) ['My', 'name', 'is', 'Nikhil']
```
4. replace : It will replace value with desired value.
```
var text = ("My name is Nikhil");
console.log(text.replace("Nikhil","Nick"));

output:
C:\Program Files\nodejs\node.exe .\nik.js
My name is Nick
```
5: trim : It is used to remove the spaces.
```
var text = ("  nikhilgotpagar1997@gmail.com  ");
console.log(text.trim());

Output:
C:\Program Files\nodejs\node.exe .\nik.js
nikhilgotpagar1997@gmail.com
```

---
### <span style="color:Gray"> 11. Built in functions & ES6.

**Functions :** 
1. setTimeout(): It delays the execution.
```

const timerfn= function(){
    console.log("print after 2 sec");
}
console.log("running 1");
setTimeout(timerfn,2000);
console.log("running 2");

Output :
C:\Program Files\nodejs\node.exe .\nik.js
running 1
running 2
print after 2 sec
```
2. setInterval(): Exactly works as a setTimeout but it runs continuously.

```
console.log("running 1");
setInterval(function(){
    console.log("print after 2 sec");
},2000);

console.log("running 2");

Output:
C:\Program Files\nodejs\node.exe .\nik.js
running 1
running 2
87
print after 2 sec
```
3.clearInterval : To clear the inetrvals.
```
console.log("running 1");
let counter = 0;

const timer=setInterval(function(){
    console.log("print after 5 sec");
    if (counter>5){
        clearInterval(timer);
    }
    counter++
},5000);

console.log("running 2");
```
5. parseInt : It converts any number into an integer value.

```
const num = 10.9;
 let intNum = parseInt(num);
 console.log(intNum);

 Output :
 C:\Program Files\nodejs\node.exe .\nik.js
10
```

---
 ![Image](https://raw.githubusercontent.com/nikhilgotpagar/METRepository/main/WhatsApp%20Image%202021-05-26%20at%2012.39.13%20PM.jpeg)







































