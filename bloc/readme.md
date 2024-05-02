bloc 의존성 주입 방법

---
---


Get_it 라이브러리


``` dart
final getIt = GetIt.instance;


  getIt.registerFactory(() => CounterBloc());

```

예를 들어:

사용자 입력 데이터
서버로부터 가져온 데이터
UI 컴포넌트의 상태 (열림/닫힘 등)
인증 정보
설정 값
등등

