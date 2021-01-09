# 조건문

## if
```c#
if(조건식 A)         // A가 참이면
{
  ...
}
else if(조건식 B)    // B가 참이면
{
  ...
}
else                // 그렇지 않다면
{

}
```

### 조건식 결과 : 참(1), 거짓(0)

### 관계 연산자 사용 : ==, !=, <, >, <=, >=

### 순서가 올바른지 확인


### 논리 연산자 : &&, ||, !


### 조건 연산자 = 삼항 연산자
- (불리언 표현식)?참의 반환값 : 거짓의 반환값
```c#
(num1 > num2)? num1 : num2;
```

### 연산자 우선순위도 있다. 찾아보자


## switch
```c#
switch(expression)
{
  case 상수 라벨1:
    codes;
    break;
  case 상수 라벨2:
    codes;
    break;
  case 상수 라벨3:
    codes;
    break;
  default:
    위에 모든 case들과 일치하지 않을 때
    break;
}
```

### break : switch 탈출

### case에 사용되는 상수형: int, long, char, bool, string
