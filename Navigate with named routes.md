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

```
onPressed
Navigator pushNamed (context, '/second')
```

### 첫번째 화면으로 gogogogogogogogoogogogogogogogo
```
onPressed
Navigator pop context

```

### 구현예


```
void main
runApp
MaterialApp
title: 'gogogogoogogog'
initialRoute: '/',
routes:
'/': (context) => const FirstScreen(),
'/second': (context) => const SecondScreen(),

class FirstScreen extends StatelessWidget
const FirstScreen super.key
@override
Widget build BuildContext context
return Scaffold
appBar: AppBar
title: const Text('첫번째 화면')
body: Center
child: ElevatedButton
onPressed:
Navigator.pushNamed(context, '/second');
child: const Text('Launch screen'),

class SecondScreen extends StatelessWidget
const SecondScreen super.key

@override
Widget build BuildContext context
return Scaffold
appBar: AppBar
title: const Text('두번째 화면')
body: Center
child: ElevatedButton
onPressed
Navigator pop(context)
child: const Text('돌아가시오~')
```
