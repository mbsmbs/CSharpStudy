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


### Property
- 컴파일러가 알아서 getter/setter 함수를 만들어준다소 생각하자
- 초기화 가능
- 기본 : public
```c#
accessMod dataType propName{accessMod get; accessMod set;} = data;
public string Owner {get; set;}
public float Gas{get; private set;} - 10.0.f;
public EGasType GasType{get; private set;}
```

## 멤버 작성 순서 :추천
1. public 멤버 변수 / 프로퍼티
2. private 멤버 변수
3. 생성자
4. public 멤버 함수
5. private 멤버 함수


## partial class
- 큰 클래스를 여러개로 쪼깨서 저장
- Human.Head.cs, Human.Hand.cs, Human.body.cs, Human.leg.cs
```c#
public partial class Human
{
   Head 관련 코드...
}


public partial class Human
{
   Hand 관련 코드...
}


public partial class Human
{
   Body 관련 코드...
}


public partial class Human
{
   Leg 관련 코드...
}
```
