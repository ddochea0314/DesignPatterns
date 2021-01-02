# DesignPatterns

The 23 Gang of Four design patterns, defined in the book "Design Patterns: Elements of Reusable Object-Oriented Software".

("Design Patterns : Elements of Reusable Object-Oriented Software"책에 정의 된 23 Gang of Four 디자인 패턴.)

## Behavioral(행위 패턴)

**1. Chain of Responsibility(책임 연쇄 패턴)**

Avoid coupling the sender of a request to its receiver by giving more then one object a chance to handle the request. Chain the receiving objects and pass the request along the chain until an object handles it.

(하나 이상의 객체에 요청을 처리 할 수있는 기회를 제공하여 요청 발신자와 수신자를 연결하지 마십시오. 수신 객체를 연결하고 객체가 처리 할 때까지 체인을 따라 요청을 전달합니다.)

>[wiki]
>객체 지향 디자인에서 chain-of-responsibility pattern은 명령 객체와 일련의 처리 객체를 포함하는 디자인 패턴이다. 각각의 처리 객체는 명령 객체를 처리할 수 있는 연산의 집합이고, 체인 안의 처리 객체가 핸들할 수 없는 명령은 다음 처리 객체로 넘겨진다. 이 작동방식은 새로운 처리 객체부터 체인의 끝까지 다시 반복된다.

**2. Command(커맨드 패턴)**

Encapsulate a request as an object, thereby letting you parameterize clients with different requests, queue or log requests, and support undoable operations.

(요청을 객체로 캡슐화하여 다른 요청, 큐 또는 로그 요청으로 클라이언트를 매개 변수화하고 실행 취소 가능한 작업을 지원할 수 있습니다.)

>[wiki]
>커맨드 패턴(Command pattern)이란 요청을 객체의 형태로 캡슐화하여 사용자가 보낸 요청을 나중에 이용할 수 있도록 매서드 이름, 매개변수 등 요청에 필요한 정보를 저장 또는 로깅, 취소할 수 있게 하는 패턴이다.

**3. Interpreter(인터프리터)**

Given a language, define a representation for its grammar along with an interpreter that uses the representation to interpret sentences in the language.

(언어가 주어지면 해당 표현을 사용하여 언어로 문장을 해석하는 인터프리터와 함께 문법 표현을 정의합니다.)

**4. Iterator(반복자패턴)**

Provide a way to access the elements of an aggregate object sequentially without exposing its underlying representation.

(기본 표현을 노출하지 않고 집계 개체의 요소에 순차적으로 액세스하는 방법을 제공합니다.)

**5. Mediator(중재자패턴)**

Define an object that encapsulates how a set of objects interact. Mediator promotes loose coupling by keeping objects from referring to each other explicitly, and lets you vary their interaction independently.

(개체 집합이 상호 작용하는 방식을 캡슐화하는 개체를 정의합니다. 중재자는 객체가 서로를 명시 적으로 참조하지 못하도록하여 느슨한 결합을 촉진하고 상호 작용을 독립적으로 변경할 수 있도록합니다.)

**6. Memento(메멘토패턴)**

Without violating encapsulation, capture and externalize an objects internal state so that the object can be restored to this state later.

(캡슐화를 위반하지 않고 나중에 개체를이 상태로 복원 할 수 있도록 개체 내부 상태를 캡처하고 외부화합니다.)

>[wiki]
>메멘토 패턴(memento pattern)은 객체를 이전 상태로 되돌릴 수 있는 기능을 제공하는 소프트웨어 디자인 패턴이다. (롤백을 통한 실행 취소) 

**7. Observer(옵저버패턴)**

Define a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.

(하나의 개체가 상태를 변경하면 모든 종속 항목에 알림이 전송되고 자동으로 업데이트되도록 개체간에 일대 다 종속성을 정의합니다.)

>[wiki]
>옵서버 패턴은 객체의 상태 변화를 관찰하는 관찰자들, 즉 옵저버들의 목록을 객체에 등록하여 상태 변화가 있을 때마다 메서드 등을 통해 객체가 직접 목록의 각 옵저버에게 통지하도록 하는 디자인 패턴이다. 주로 분산 이벤트 핸들링 시스템을 구현하는 데 사용된다.

**8. State(상태패턴)**

Allow an object to alter its behavior when its internal state changes. The object will appear to change its class.

(내부 상태가 변경 될 때 개체가 동작을 변경할 수 있도록합니다. 개체가 클래스를 변경하는 것처럼 보입니다.)

**9. Strategy(전략 패턴)**

Defines a family of algorithms, encapsulates each one, and make them interchangeable. Strategy lets the algorithm vary independently from clients who use it.

(알고리즘 제품군을 정의하고 각 알고리즘을 캡슐화 한 다음 상호 교환 가능하게 만듭니다. 전략을 사용하면 알고리즘이이를 사용하는 클라이언트와 독립적으로 달라질 수 있습니다.)

**10. Template Method(템플릿 메소드 패턴)**

Define a skeleton of an algorithm in an operation, deferring some steps to subclasses. Template Method lets subclasses redefine certain steps of an algorithm without changing the algorithms structure.

작업에서 알고리즘의 골격을 정의하여 일부 단계를 하위 클래스로 연기합니다. 템플릿 메서드를 사용하면 하위 클래스가 알고리즘 구조를 변경하지 않고도 알고리즘의 특정 단계를 재정의 할 수 있습니다.

>[wiki]
>템플릿 메소드 패턴은 소프트웨어 공학에서 동작 상의 알고리즘의 프로그램 뼈대를 정의하는 행위 디자인 패턴이다. 알고리즘의 구조를 변경하지 않고 알고리즘의 특정 단계들을 다시 정의할 수 있게 해준다. 

**11. Visitor(비지터 패턴)**

Represent an operation to be performed on the elements of an object structure. Visitor lets you define a new operation without changing the classes of the elements on which it operates.

(개체 구조의 요소에 대해 수행 할 작업을 나타냅니다. 방문자를 사용하면 작동하는 요소의 클래스를 변경하지 않고 새 작업을 정의 할 수 있습니다.)

>[wiki]
>객체 지향 프로그래밍과 소프트웨어 공학에서 비지터 패턴은 알고리즘을 객체 구조에서 분리시키는 디자인 패턴이다. 이렇게 분리를 하면 구조를 수정하지 않고도 실질적으로 새로운 동작을 기존의 객체 구조에 추가할 수 있게 된다. 개방-폐쇄 원칙을 적용하는 방법의 하나이다.

## Creational(생성 패턴)

**12. Abstract Factory(추상팩토리패턴)**

Provide an interface for creating families of related or dependent objects without specifying their concrete classes.

(구체적인 클래스를 지정하지 않고 관련되거나 종속 된 개체의 패밀리를 만들기위한 인터페이스를 제공합니다.)

**13. Builder(빌더패턴)**

Separate the construction of a complex object from its representation so that the same construction processes can create different representations.

(복잡한 객체의 구성을 표현에서 분리하여 동일한 구성 프로세스가 다른 표현을 만들 수 있도록합니다.)

**14. Factory Method**

Define an interface for creating an object, but let the subclasses decide which class to instantiate. Factory Method lets a class defer instantiation to subclasses.

**15. Prototype**

Specify the kinds of objects to create using a prototypical instance, and create new objects by copying this prototype.

**16. Singleton**

Ensure a class only has one instance, and provide a global point of access to it.

## Structural

**17. Adapter**

Convert the interface of a class into another interface clients expect. Adapter lets classes work together that couldn't otherwise because of incompatibility interfaces.

**18. Bridge**

Decouple an abstraction from its implementation so that the two can vary independently.

**19. Composite**

Compose objects into tree structures to represent part-whole hierarchies. Composite lets clients treat individual objects and compositions of objects uniformly.

**20. Decorator**

Attach additional responsibilities to an object dynamically. Decorators provide a flexible alternative to subclassing for extending functionality.

**21. Facade**

Provide a unified interface to a set of interfaces in a system. Facade defines a higher-level interface that makes the subsystem easier to use.

**22. Flyweight**

Use sharing to support large numbers of fine-grained objects efficiently. A flyweight is a shared object that can be used in multiple contexts simultaneously. The flyweight acts as an independent object in each context. It is indistinguishable from an instance of the object that is not shared.

**23. Proxy**

Provide a surrogate or placeholder for another object to control access to it.
