# Exception
- try/catch
- try 블록 안에 마지막 줄까지 문제없이 실핼 되면 catch블록 실행안됨
- 예외가 발생하면 try 블록 안의 모든 코드를 건너뛰고
  - 해당 예외 상황을 처리하는 catch문이 있다면 이 안에서 해경
  - catch문이 없으면 호출자에게 throw
- catch블록은 여러개가 있을 수 도 있고 순서대로 평가

## Exception class
```c#
catch(Exception e)
catch(FileNotFoundException e)
```

### 여러 프로퍼티, 함수가 있다.

### 파일을 열었으면 닫는거 잊지 말자
```c#
try
{
  ...
}
catch(IOException e)
{
  ...
}
finally
{
  ...
}
```

## Custom  Exception
- 나만의 예외를 만들 수 있다.
- 하나의 클래스다
- Exception 상속 받아야함
1. 새로운 XxxException.cs 파일을 만든다.
2. Exception 상속
3. 생성자 추가
```c#
public XxxException(string message)
  : base(message)
{
  if(..)
  {
    throw new XxxException("...");
  }
}
```
