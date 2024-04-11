
```
```

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
