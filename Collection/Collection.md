# Collection
- 자료구조
- 동일한 형의 여러 자료를 저장하는 공간
- 각 자료구조마다 다양한 메서드들이 있다.

## 1. List
- 배열과 비슷
- 요소 수를 언제나 바꿀 수 있다.
```c#
List<T> listName = new List<T>();   // T : generic == C++ template programming

List<int> scores = new List<int>();

List<int> scores = new List<int>(3);
```


## 2. Dictionary
- TKey : 어떤 자료형의 키
- TValue : 어떤 자료형의 값
```c#
Dictionary<TKey, TValue> DictName = new Dictionary<TKey, TValue>();

Dictionary<string, int> myDict1 = new Dictionary<String, int>();
```


## 3. Hash Set
- 딕셔너리랑 비슷
- 키만 있다.
```c#
HashSet<T> setName = new HashSet<T>();

HashSet<int> studentIDs = new HashSet<int>();
```
