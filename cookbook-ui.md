## Q. How to add gradient as a color background?
Ans . 
1. Take ```Container``` widget
2. use ```decoration``` property of ```Container```.
3. you can use ```BoxDecoration``` object instance.
4. use ```gradient``` property of ```BoxDecoration```, u can use ```LinearGradient()``` instance.

e.g.
```
...
body: Container(
          decoration: const BoxDecoration(
              gradient: LinearGradient(
                  begin: Alignment.topCenter,
                  end: Alignment.bottomRight,
                  colors: [Colors.red, Colors.pink, Colors.purple])),
...
```
*****
## Q. 
   
