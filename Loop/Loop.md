# 반복문

## for
```c#
for(몇부터; 몇까지; 얼마씩 더하며)
{
  ...
}

for(int i = o; i < 3; ++i)    // 0부터 2 까지 1씩 더하며 반복
{
  ....
}
```

## while
```c#
while(조건식)      // true면 반복
{
  ...
}

while(count < 3)    // count가 3보다 작을 동안에 반복
{
  ...
}
```

### break : 탈출
```c#
if(passcode = userInput)    // 어떤 조건이 충족되면
{
  codes...;                 // 코드가 있다면 실행하고
  break;                    // 반복문 탈출
}
```

### continue : 무시
```c#
if(passcode = userInput)    // 어떤 조건이 충족되면
{
  continue;                 // 이번횟수 무시하라
}
```
