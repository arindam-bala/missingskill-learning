> # **JavaScript**
---
> ## **Contents**
---
[History](#History)

[Data Types](#Data-Types)

[Variables](#Variables)

[Function](#Function)

[Objects](#Objects)

[Mind Map](#Mind-Map)

---
> ### **History**

---
[Contents](#Contents)
1. JavaScript was developed by Brenden Eich in 1995 when he worked in Netscape Communications.


1. That time Netscape Navigator was worlds most popular browser.


1. In 1995 Microsoft also launched Internet Explorer internet browser to break Netscape's monopoly in the field of internet browser.
Because Netscape's browser was a paid software. 

1. Netscape's internet browser was called Netscape Navigator back then.

1. Later the name of this language was changed to LiveScript.

1. After coming Internet Explorer from Microsoft, Netscape's monopoly was breakdown. Because Internet Explorer was totally free.

1. In Netscape Navigator browser all the front end part was controlled by the language LiveScript back then. 
 
1. In the back end of this Netscape Navigator an another language works. This is also a very popular language at present time. The name of the language is Java. 

1. Java was an Object Oriented Programming Language and developed by Sun Microsystems.

1. Java was not totally compatible to the Netscape Platform. So a totally new kind of programming language was developed within three weeks and it is called Mocha back then.

1. After that Netscape, Mocha and Livescript together changed the name of the language to JavaScript. 

1. JavaScript was totally a front end language back then. And Java was patented and copyrighted  by Sun Microsystems for the back end processing.

1. The name was given JavaScript because of getting popularity. Because Java was a popular language back then.

1. In 1996 Google started. Totally based on JavaScript.
---

> ### **Data Types**

---
[Contents](#Contents)

**Storing data is a very essential part of every  programming language. Variables are the places where data are stored. For storing different types of data, variables have to be of different types also. This types are known as Data Types in variables.**

* JavaScript have several data types
    
    * **Primitive Data Types** : Primitive data types are not object and has no methods .

        * boolean
        * null
        * number
        * String
        * symbol
        * undefined
    
    * **Composite Types**: Composite types are also primitive types but into some larger structure. In JavaScript object is the main composite data type and from **Object** all other composite types are evolved.

    **It is also called Copy By Reference** 
        
        * objects
        * arrays

---
> ### **Variables**
---
[Contents](#Contents)

In JavaScript there are three kinds of variable declarations.

---

* **var** : it is the normal declaration of a variable.

    * Example:

    ```JavaScript   
        <script>
            var myName = "Arindam";
            var myID = 32596;
            console.log(myName);
            console.log(myID);
        </script>   
    ```

---

* **let** : This is a local variable. This variable's scope is blocked by scope rules.
This is actually a local variable.
 
* Example:
    
```JavaScript
        <script>
            let a = 1;
            if (a === 1) {
            let a = 2;
            console.log(a);
            // expected output: 2
            }
            console.log(a);
            // expected output: 1
        </script>
```

---

* **const** : It is also a block scoped variable. But it is totally Read Only.

* Example:

```JavaScript
    <script>
        const a = 10;
        a = 20; //error
        console.log(a);
        //10
    </script>
```
---

> ### **Function**
---
[Contents](#Contents)

Function in JavaScript is a set of instructions for performing a specific task. It is also known as procedure. To use a function first we have to define it in a scope from which we wish to call it.

* Example:
 ### **This is also an example of primitive parameter passing to a function**


```JavaScript
        <script>
            var num1 = 5;
            var num2 = 4;
            function rectArea(num1,num2){
                return num1 * num1;
            }
            console.log(rectArea);
        </script>
```
This is a simple representation of a function. Here function rectArea takes num1 and num2 as function arguments and calculate the result inside the function body. It returns the result. This is the function defination and declaration. 

**In console.log(function name)**  we just call the function to perform its task. 

---
### Scopes of Function
---
[Contents](#Contents)

* Scope of function means working and accessing area of a function. It depends on where we define and call a function. This is also applicable for variables declaration in program.

* A variable which is defined globally can be accessed from anywhere of the program. But variables declared inside a function cannot be accessed outside the function. 

* A funtion can be defined and called inside of another funtion. This is called nesting of functions.

**A example is given below.**

    
```JavaScript
        <script>
            // global variables
            var num1 = 16;
            var num2 = 4;
            var name = 'Arindam';

            // globallly declared function
            function multiply(){
                return num1 * num2;
            }

            multiply(); 
            // function calls returns value 64

            // nesting of a function
            function getValue() {
            var num1 = 2,
            num2 = 3;

            function add() {
                return name + ' gets ' + (num1 + num2);
            }

            return add();
            }

            getValue(); // function calling gives output

        </script>
```

---
### **Non Primitive Parameter Passing of a Function**
---
[Contents](#Contents)


In this section we will see how a function takes a non primitive parameter as an argument.
    
* Example:

```JavaScript
    <script>
        function test(arr){
            var a = arr;
            return a;
        }
        var array = [1,2,3,4,5];
        console.log(test(array));

    </script>
```
The above example takes the array as an argument to the function test and prints output.




---
* ## **Types of function in JavaScript**:



    1.**Inline Function** : This is a anonymous function assigned to a variable.

    * Example:

    ```
        var fun = function(){

        }
    ```
    ---
    
    1. **Higher Order Function** :

    --- 


    1. **Pure Function** : Pure functions means normal function. Which takes values as arguments and does not change it. Just processing it according to its given instructions. The output of this funtion cannot be changed.

        * Example

        ```JavaScript
            <script>
                function mult(m,n){
                    return m * n;
                }
                var a = 2;
                var b = 3;
                const data = mult(a,b);
                console.log(a,b);
                console.log(data);
            </script>
        ```

        ---  
   
    1. **Arrow Function** : It is an compact alternative of a normal traditional function expression. Uses of this function is limited and can't be applied in every situations.

        * Example:

        ```JavaScript
            <script>
                (a) =>{
                    return a + 10;
                }
            </script>
        ```

        ---
    1. **IIFE(Immediately invoked function Expression)**:  Function that runs immediately after defined.

        * Example:

        ```JavaScript
            <script>
                (function(){
                    //function body
                    let variableOne;
                    let variableTwo;
                })();
            </script>
        ``` 
        Those variables inside the function will be discarded immediately after the function is executed.
    


---    

> ### **Function Returning a Function**
---

[Contents](#Contents)

This is one kind of generating one function inside another function.

* Example:
 
 ```JavaScript
    <script>
        function test1(a,b){
            var m = a;
            var n = b;
            function test2(){
                var c = m + n;
            }
            return(test2);
        }

        console.log(test1(2,3));
    </script>

 ```
 Here the function test1 returns function test2.

 ---

 > ### **Objects**
 ---
 [Contents](#Contents)

 1. In JavaScript, an object is an unordered set of properties. It is accessed with the help of a dot(.) opetator.

1. It is like a glass. A glass has its own properties. Like its color, build material, size etc.

1. An object can hold many primitive type as well as non primitive data types.

    * Example:

    ```JavaScript
        <script>
            var myComputer ={
                "name": "Lenovo G50-80"
                "brand": "Lenovo"
                "memory": "8GB"
                "storage": "240GB"
                "processor": "Core i5" 
            }
        </script>
    ```    
In the given piece of code **"name"** ,**brand** etc are the properties of the object **myComputer**.

---
* ### Accessing Values of an Object
---
[Contents](#Contents)

* Example:

```JavaScript
        <script>
            var myComputer ={
                "name": "Lenovo G50-80"
                "brand": "Lenovo"
                "memory": "8GB"
                "storage": "240GB"
                "processor": "Core i5" 
            }
            var nameValue = myComputer.name;
            var brandValue = myComputer.brand;
            var memValue = myComputer.memory;
            var strValue = myComputer.storage;
            var proValue = myComputer.processor;

            console.log(nameValue);
            console.log(brandValue);
            console.log(memValue);
            console.log(strValue);
            console.log(proValue);
        </script>

```
This small piece of code can print the values inside the poroperties of the object **myComputer**.

---
> ### **Mind Map**
---
[Contents](#Contents)

* ## JavaScript
    
    * **History**
        
        * 1995
        * Earlier Design Mocha,Live Script
        * Designed by Brendon 
        * Donated to ECMA to create a standard implementation

        * New JS is based on ECMAScript
        * JavaScript = Java + LiveScript
    
    * **Browsers**
        
        * Chrome
        * Brave
        * Mozilla Firefox
        * Edge
        * Opera
        * Safari

    * **Variables**

        * Are Containers
        * Categories
            
            * Primitive
            * Non Primitive
        * Data Types
            
            * number
                
                * number prototype
            * boolean

                * boolean prototype
            * string
                
                * string prototype
            * undefined
            * null
            * symbol(ES6)

                * symbol
            * array

                * array prototype
            * object

                * object prototype

    * **Tech Debt**

        * plus symbol(+)

            * Acts as concat and depending on variable type

            * Always do concat when one variable is string type

        * ===(strictly equal symbol)

            * Identify, type check
        * null
            
            * Missed if check of null type
            (returns a type of object)

    * **declaration** 

        * ES5

            * var

                * functional scope

                    * local
                    * global scope

        * ES6

            * let
            * cost

---
[Contents](#Contents)

/* END OF DOCUMENT*/




    
   



        

















