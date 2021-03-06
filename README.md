# HeadFirst DesignPattern

<h1>디자인 패턴의 소개</h1>

<h3>1. 옵저버 패턴</h3>
뭔가 중요한 일이 일어났을 때 객체들한테 새소식을 알려줄 수 있는 패턴이 있다. 객체 쪽에서는 정보를 받을지 여부를 실행중에 결정할 수 있다. 옵저버 패턴은 JDK에서 가장 많이 쓰이는
패턴 가운데 하나다. 일대다 느슨한 결합에 대해 장점을 가지고 있다.

출판사 + 구독자 = 옵저버 패턴
신문 구독 메커니즘만 제대로 이해할 수 있다면 옵저버 패턴을 쉽게 이해 할 수 있다.
출판사를 주제(subject), 구독자를 옵저버(observer)라고 부른는 것만 외우자.
        

옵저버패턴에서는 한 객체의 상태가 바뀌면 그 객체에 의존하는 다른 객체들한테 연락이 가고 자동으로 내용이 갱신되는 방식으로 일대다 의존성을 정의한다.
한 객체의 상태가 변경되면 그 책체에 의존하는 모든 객체에 연락이 간다.

주제 역할을 하는 구상 클래스에서는 항상 subject 인터페이스를 구현해야 한다. 주제 클래스에서는 등록 및 해지를 위한 메소드 위에 상태가 바뀔 때마다 모든 옵저버들에게
연락을 하기 위한 notifyObservers()메소드도 구현해야한다.

옵저버가 될 가능성이 있는 객체에서는 반드시 Observer 인터페에이스를 구현해야한다. 이 인터페이스에는 주제의 상태가 바뀌었을때 호출되는 update() 메소드 밖에 없다.

Observer 인터페이스만 구현한다면 무엇이든 옵저버 클래스가 될 수 있다. 각 옵저버는 특정 주제 객체에 등록을 해서 연락을  받을 수 있다.

데이터의 주인은 주제(Subject)이다. 옵저버는 데이터가 변경되었을 때 주제에서 갱신해 주기를 기다리는 입장이기 때문에 의존성을 가진다고 할 수 있다. 이런 방법을 사용하면 여러
객체에서 동일한 데이터를 제어하도록 하는 것에 비해 더 깔끔한 객체지향 디자인을 만들 수 있다.

두 객체가 느슨하게 결합되어 있다는 것은, 그 둘이 상호작용을 하긴 하지만 서로에 대해 서로 잘 모른다는 것을 의미한다.
옵저버 패턴에서는 주제와 옵저버가 느슨하게 결합되어 있는 객체 디자인을 제공한다.
1. 주제가 옵저버에 대해서 아는 것은 옵저버가 특정 인터페이스를 구현한다는 것 뿐이다.
2. 옵저버는 언제든지 새로 추가할 수 있다.
3. 새로운 형식의 옵저버를 추가하려고 할 때도 주제를 전혀 변경할 필요가 없다.
4. 주제와 옵저버는 서로 독립적으로 재사용할 수 있다.
5. 주제나 옵저버가 바뀌더라도 서로한테 영향을 미치지 않는다.

옵저버 패턴을 코드에 적용시키는 방법을 고민해보자!

<h3>2. 데코레이터 패턴</h3>
<h3>3. 팩토리 패턴</h3>
<h3>4. 싱글턴 패턴</h3>
<h3>5. 커맨드 패턴</h3>
<h3>6. 어댑터 패턴, 퍼사드 패턴</h3>
<h3>7. 탬플릿 메소드 패턴</h3>
<h3>8. 이터레이터와 컴포지트 패턴</h3>
<h3>9. 스테이트 패턴</h3>
<h3>10. 프록시 패턴</h3>
<h3>11. 컴파운드 패턴</h3>
<h3>12. 팩토리 패턴</h3>
