


### login_screen.dart 수정사항

```
import material, myproj path
class signupscreen extends statefulwidget
static const string routename = /signup


@override
_signupscreenstate createstate()=>_signupscreenstate

class _signupscreenstate extends state signupscreen
final globalkey formstate _formkey = globalkey formstate

final texteditingcontroller _emailcontroller = texteditingcontroller
...

void initstate
super initstate

void dispose
_emailcontroller dispose

@override
widget build buildcontext context
return scaffold
body safearea
chil form
key _formkey
child listview
padding const edgeinsets symmetric horizontal 20.0
children widget

logintextfield
controller _emilcontroller
labetext 이메일
validator value
if value == null || value isempty
return 이메일입력
return null

logintextfield
...

elevatedbutton
onpresssed
if _formkey.currentstate! validate
child text 회원가입
```



#### 0411수업노트
```



Textbutton

Onpressed
_emailkey.currentstate? validate()

Child
Const text
‘회원가입


GestureDetector
- 체스처 동작 감지
inkwell

singup folder - singup_screen.dart
stl
Return scaffold
Body safe area
child column
loginTextField context con

Network connection



Class app screen static string signup=‘’/singUp
-> 경로 지정 방법

stf위젯
Controller- 5개
Email, pw,pwconfirm,name,stn(student number)

Initstate에 초기화


Void initstate

List<(TextEditingController, String)> get _buttons => [(),(),(),(),(),()]


listview.separated
Itemcount _buttons.length 10.heightbox
Item builder context index
Var button=_buttons[index];

Return logintextfield
Controller button.$1
Labeltext buton.$2



Class logintextfield extends stateless widget
Final globally form state? formkey
Final bool obscure text

Final string? Function string? ? validator

obscuretext true 

Const logintextfield
Super key
This formkey
This.obscuretext = false


Const logintextfiled

Widget build build context context
Return

Controller controller
Ontapoutside event

Focusmanager instance primaryfocus

Return logintextfield
Key
Controller
Labeltext

Validator value
If value == null || value.isEmpty
Return 값 입력
If button $3 == 이름
If value length != 3
Return 정확한 이름 입력


Var check email - _emailkey.currnetstate?,validate ?? false


If !checkemail || …
Return


login_screen.dart ->
Body jsonencode
Email email
Password pw
Name name
Student_number stn

http:175.197.109.158:60080





```
