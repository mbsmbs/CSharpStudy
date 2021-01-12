# OOP
- Object = State + Behaviour

## Class
- 멤버 변수의 기본값 : 0
- 참조형의 기본 값 : null
```c#
accessModifier class className
{
  accessModifier memberVar;
  accessModifier memberMethod(...)
  {
    ...
  }
}

className varName = new className();  // 개체 만들기
```

### 생성자
- 개체를 만들면 자동으로 호출되는 함수
- 클래스와 이름이 같은 함수
- 멤버 변수 초기화
- 생성자가 여러개일 수도 있다.
```c#
public class Car
{
  public int price;

  public Car(int price)
  {
    price = price
  }
}
```

### 접근 제어자
- public : 누구라도 접근 가능
- private : 클래스 안에서만 접근 가능
- protected
- internal
