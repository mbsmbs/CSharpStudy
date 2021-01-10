# 함수

## 함수 정의
```c#
dataType functionName(parameters)
{
  codes...
  return something;                 // 반환형이 void가 아닌경우 반드시 return
}

/* 사용 */
dataType dataname = functionName(parameters);
.
.
.
```

### 메인 함수의 매개변수에 데이터 넘기는 법
- 비주얼 스튜디오에서 프로젝트 우클릭 -> 디버그 -> 응용 프로그램 인수에 입력

### 배열의 길이 : Length (property)
```c#
string[] args;

int length = args.Length;     // arrayName.Length
```

## 함수와 범위 {}
- 안에서는 밖에 있는 데이터 접근 가능 밖에서는 불가능
- 함수 안에 선언한 모든 것은 그 함수에서만 사용 가능 ( 지역변수 )


## 값에 의한 전달, 참조에 의한 전달
- 값   : 매개변수에 변수의 사본을 전달
- 참조 : 매개변수에 변수의 원본을 전달 (ref 사용)
```c#
int something(ref int data)
{
  ...
}
```
