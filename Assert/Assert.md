# Assert
- 코드 검증을 위한 코드
- 절대로 발생하지 않아야 하는 조건을 런타임 중에 검사
- 함수의 선조건 검사에 쓰기 적당
- 디버그 모드에서만 동작
- 릴리즈 모드에서는 무시

```c#
using System.Diagnostics;

Debug.Assert(condition);          // condition안에 false면 어써트 발생 일시 중단
Debug.Assert(condition, "msg");   // condition안에 false면 일시 중단되고 msg 출력
```
