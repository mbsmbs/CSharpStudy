# 열거형
- 정수형 상수의 집합
- 각 원소마다 고유의 이름을 가짐
- 집합 역시 고유의 이름을 가짐
- enum은 변수로 사용 가능
- 정의는 함수 밖에서
- 첫 번째 원소의 기본값은 0 
- 아무값도 대입하지 않으면 1씩 증가
- 부동 소수점 안됨
- 가독성에 좋음
- 함수에 다른 값이 들어가면 컴파일 오류
- const < enum

```c#
enum EDirection
{
  North,  // 0
  South,  // 1
  East,   // 2
  West    // 3
};

/* 직접정의 */
enum EDirection
{
  North = 5,
  South = 10,
  East = 15, 
  West = East + 10   
};

enum EDirection
{
  North = 5,
  South,      // 6
  East,       // 7
  West        // 8
};
```
