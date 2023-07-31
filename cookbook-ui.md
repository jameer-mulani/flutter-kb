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
## Q. How to lock the screen orientation in flutter?
Ans.
1. for locking the orientation one can use the below code:
   ```
    //Ensuring is must
    WidgetsFlutterBinding.ensureInitialized();

    //SystemChrome utility class allows to set preferred orientation.
    SystemChrome.setPreferredOrientations([
     //specify list of preferred orientation
    DeviceOrientation.portraitUp
    ]).then((value) => {
      //call your runApp() once future is returned.
             runApp(app);
    });
   ```
*****
## Q. How to know the current screen orietation in flutter?
Ans.
1. We can use ```MediaQuery``` class for this.
   ```
   MediaQuery.of(context).orienation == Orientation.portrait
   ```
*****
## Q.How to know the current screen size in flutter?
1. use ```MediaQuery``` class for this.
   ```
   final width = MediaQuery.of(context).size.width;
   final height = MediaQuery.of(context).size.height;
   ```
*****
## Q.
