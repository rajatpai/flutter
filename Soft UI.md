# Soft UI

<p align="center">
<img src="https://imgur.com/h9yjSAv.png" width = 750>
</p>

```dart
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner : false,
      home : Home(),
    );
  }
}

class Home extends StatefulWidget {
  @override
  _Home createState() => _Home();
}

class _Home extends State<Home>{
  @override
  Widget build(BuildContext context){
    return Scaffold(
      backgroundColor : Colors.amber[300],
      
      body : Center(
        child : Container(
          width : 200,
          height : 200,
          child : Icon(Icons.android, size: 80,),
          decoration : BoxDecoration(
            color :  Colors.grey[300],
            borderRadius : BorderRadius.all(Radius.circular(50)),
            boxShadow : [
              BoxShadow(
                color: Colors.grey,
                offset: Offset(4.0, 4.0),
                blurRadius : 15.0,
                spreadRadius : 1.0,
              ),
              BoxShadow(
                color: Colors.amber,
                offset: Offset(-4.0, -4.0),
                blurRadius : 15.0,
                spreadRadius : 1.0,
              ),
            ]
          ),
        ),
      ),
    );
  }
}
```
