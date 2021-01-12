# String Builder
- 무자열을 효율적으로 만들어주는 라이브러리(클래스)
- 동작 :
  - 긴 문자열을 담을 수 있는 충분한 공간을 미리 확보
  - 추가되는 문자열들로 그 공간을 차례대로 채워 나감
  - 모든 것이 준비되면 최종적으로 문자열을 만들어서 반환

```c#
StringBuilder varName = new StringBuilder(int maxCharCount);  // maxCharCount만큼 StringBuilder를 생성
```

## 다양한 메서드들이 있다
- AppendLine(string text);
- Append(string text);
- ...
