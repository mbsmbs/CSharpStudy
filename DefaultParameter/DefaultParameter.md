# 기본값 인자
- 함수 선언할 때 기본 값을 정해둘 수 있다.
- 하나 이상 가능
- 나중에 중간에 추가할 때 문제가 생길 수 있으니 주의, 맨뒤에 추가하자
- 기본값은 0으로 하자
```c#
static string GetHP(int level, int mapID, int difficulty = 0, string name);   // compile error

static string GetHP(int level, int mapID, string name, int difficulty = 0 );   // ok
```
