# Demo 1
--- 

# Demo 2
- How to remove debug 
- How to change the theme color
- How to style the container more
- How to extract an element

Styling example

```dart
import 'package:flutter/material.dart';

void main(){
runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: HomePage(),
    );
  }
}

class HomePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Center(
        child: Container(
          height: 200.0,
          width: 200.0,
          decoration: BoxDecoration( 
            color: Colors.blueAccent,
            border: Border.all(
              color: Colors.black,
              width: 2.0,
            ),
            borderRadius: BorderRadius.circular(10.0),
            gradient: const LinearGradient(
              colors: [
                Colors.black,
                Colors.greenAccent
              ]
            ),
            boxShadow: const [
              BoxShadow(
                color: Colors.grey ,
                blurRadius: 2.0,
                offset: Offset(2.0,2.0)
              )
            ]
          ),
        ),
      ),
    );
  }
}
```
