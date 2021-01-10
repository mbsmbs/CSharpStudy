# 재귀함수
- 작은 문제를 해결하고 그것을 이용해 더 큰 문제를 해결
- 종료 조건 (base case) + 재귀 함수 호출

## 피보나치 수열 : 0 1 1 2 3 5 8 13 21 34 55 ....
```c#
public static int FibonacciRecursive(uint number)
{
  if(number == 0)
  {
    return 0;
  }
  
  if(number == 1)
  {
    return 1;
  }
  
  return FibonacciRecursive(number - 2) + FibonacciRecursive(number - 1);
}
```

## 하노이의 탑
- 한 번에 원판 하나씩만 옮길 수 있음
- 작은 원판 위에 그보다 큰 원판을 옮길 수 없음

### 풀이
- 막대 3개가 있고, 어느 한 막대에 n개의 원파이 있음
- n개의 원판에서 상위 n-1개를 다른 막대에 옮길 수 있다고 가정
- n-1개의 원판을 중간 막대로 옮김
- 마지막 n번째 원판은 목적지 막대에 옮김
- 중간 막대에 있던 n-1개의 원판을 목적지 막대에 옮김
- 이걸 n-2, n-3,..base case까지 반복
