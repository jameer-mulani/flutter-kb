### About Dart:
- Dart has been created by Google in early 2013 initially for Chrome browser but gains its popularity in 2018 when Flutter introduced to the world.
- Dart is highly optimised application design language unlike Go, C or C++ which are system design languages.
- Dart help faster development and execution with its flexible adoption to both ***JIT(Just in Time)*** and ***AOT(Ahead of Time)*** compilation
- When dart runs in development it uses JIT and when compile to ARM then it uses AOT which gives it almost native like running performance.
- Statement is Dart ends with semicolon(;).


### Type System:
- ```var``` is type to define to the varible and once the assignment is done with the value then actual type gets infered or derived
  ```var a = 3;```
- Type int and value 3 is assigned, later one can not changed to some other value
- Flutter support ```int``` and ```double``` to represent the number there is no such type like byte, short or float, dart memory optimisation allocate right memory for type smaller than ```int``` or ```double```
- Dart has ```num``` type as well which is superset of ```int``` and ```double```
- Dart has ```String``` to represent the string, one can use singlequoute or doubleqoute to create string literal, expression in the string are evaluated using ```$``` or ```${}``` syntax

### Functions:
- Dart has similar notion of function like any other famous languges like function in dart has return type, function name, parameter list, body and return expression.
-   ```
    String getName(int id){
        //function body
      return userRepository.getUserById(id).name;
    }
    ```
- If function is single exression statement as a body then consise sytax is used by fat arrow ***=>***
- ```
  final pi = 3.14;
  double doubleThePiWith(int p) => p * pi *2;
  ```
- ambda are the unnamed function with optional parameter list but body assigned to varible.
- Due to support of lambda expression function in the Dart becomes the higher order function, higher order function are those functions in the programming language which can be called like normal function howerver one can pass other function as a paramter to it and can return the function from it.
-  one liner function lambda syntax is like this ***(<parameters>)=><Expression>***
-  ```
    Function foo = (double x)=> x*x;
   
     main(){
       var result = foo(3.14);
       print(result);
     }
   ```
- Multiline lambda syntax is like this ***(<parameters>){ //body   return expression;}***
- ```
   Function bar = (dobule x){
    assert(x is double);
    double value = x * x;
    reurn value;
   };
  ```
