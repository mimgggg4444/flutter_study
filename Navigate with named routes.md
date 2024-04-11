```

```

### 화면 2개 만들기

```
import 'package:flutter/material.dart';

class FirstScreen extends StatelessWidget
const FirstScreen super.key

  @override
  Widget build BuildContext context 
  return Scaffold
  appBar AppBar
  title const Text First Screen
  body Center
  child ElevatedButton
  onPressed
  child const Text Launch screen
  

class SecondScreen extends StatelessWidget
const SecondScreen super.key
  @override
  Widget build BuildContext context
  return Scaffold
  appBar AppBar
  title const Text Second Screen
  body Center
  child: ElevatedButton
  onPressed
  child const Text Go back
```
  
        
### 경로설정


```
MaterialApp
title Named Routes Demo
initialRoute '/'
routes

'/': (context) => const FirstScreen()
'/second': (context) => const SecondScreen(),
```

### 두 번째 화면으로 이동

