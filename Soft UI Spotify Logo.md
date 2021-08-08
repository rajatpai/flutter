# Spotify Logo

<p align="center">
<img src="https://imgur.com/ake1u2t.png" width = 750>
</p>


```dart
import 'package:flutter/material.dart';
import 'dart:math';

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
      backgroundColor : Colors.grey[800],
      
      body : Center(
        child : Container(
          width : 200,
          height : 200,
          child : Transform.rotate(
            angle: 269 * pi / 180,
            child: Icon(Icons.contactless, size: 80, color : Colors.lightGreenAccent[700],),
            ),
          decoration : BoxDecoration(
            color :  Colors.black,
            borderRadius : BorderRadius.all(Radius.circular(50)),
            boxShadow : [
              BoxShadow(
                color: Color(0xFF212121),
                offset: Offset(4.0, 4.0),
                blurRadius : 15.0,
                spreadRadius : 1.0,
              ),
              BoxShadow(
                color: Color(0xFF616161),
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
