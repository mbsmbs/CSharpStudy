# 함수 오버로딩
- 동일한 함수이름, 다른 매개변수

## 언제 사용할까?
1. 매개변수의 수가 다른경우 사용

2. 승격/묵시적 변환을 해도 상관 없는 경우

3. 매개변수가 아예 승격이 불가능한 경우
```c#
static double Sqrt(double num){...}
static double Sqrt(int num){...}
```
