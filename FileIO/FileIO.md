# 파일 입출력
```c#
using System.IO
```

## 여러 함수들이 있음
- 텍스트 파일 저장, 덧붙히기, 쓰기, 읽기...
- 이진 파일 전용...

## 파일이 존재하지 않으면 exception


# FileStream
- 메모리 부담을 덜어주기 위해 일부만 읽어온다
- 예: 웹 브라우저에서 이미지 뜰 때 한번에 뜨지 않고 점점 뜨는 경우
- 여러 함수, 프로퍼티가 있다.
- Open하면 Close 잊지 말자

## using
- 알아서 Close()해줌
- using문을 사용해야 할 때:
  1. 클래스 헤더에 IDisposable이 있으면
  2. 멤버 함수가 Dispose()가 있으면

```c#
using(...)
{
  ...
}
```
