# LINQ
- 데이터베이스 쿼리문처럼 비슷하게 사용할 수 있다

## 같은 코드
```c#
using System.Linq;

var filteredItems = from item in menuItems
                    where item.Price > 15
                    select item;
```
```c#
SELECT * FROM MenuItems
where price > 15;
```

## 여러가지 함수들이 있다.
