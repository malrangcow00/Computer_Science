### 디자인 패턴
- 모듈 간의 관계 및 인터페이스를 설계할 때 참조할 수 있는 전형적인 해결 방식 또는 예제
- 문제 및 배경, 실제 적용된 사례, 재사용이 가능한 샘플 코드 등으로 구성
- 개발 과정 중에 문제가 발생하면 새로 해결책을 구성하는 것보다 문제에 해당하는 디자인 패턴을 참고하여 적용하는 것이 더 효율적
- GOF의 디자인 패턴은 생성 패턴, 구조 패턴, 행위 패턴으로 구분

### 생성 패턴 (Creational Pattern)
- 클래스나 객체의 생성과 참조 과정을 정의하는 패턴
<table>
<tr>
<td>
추상 팩토리<br>
(Abstract Factory)
</td>
<td><li>구체적인 클래스에 의존하지 않고, 인터페이스를 통해 서로 연관/의존하는 객체들의 그룹으로 생성하여 추상적으로 표현</li><li>연관된 서브 클래스를 묶어 한 번에 교체하는 것이 가능</li></td></tr>
<tr>
<td>빌더<br>
(Builder)</td>
<td>
<li>작게 분리된 인스턴스를 건축 하듯이 조합하여 객체를 생성</li>
<li>객체의 생성 과정과 표현 방법을 분리하고 있어, 동일한 객체 생성에서도 서로 다른 결과를 만들어낼 수 있다</li></td></tr>
<tr><td>
팩토리 메소드<br>
(Factory Method)
</td>
<td><li>객체 생성을 서브 클래스에서 처리하도록 분리하여 캡슐화한 패턴<li>상위 클래스에서 인터페이스만 정의하고 실제 생성은 서브 클래스가 담당</li>
<li>가상 생성자(Virtual Construtor) 패턴이라고도 한다</li></td>
</tr>
<tr>
<td>프로토타입<br>
(Prototype)</td>
<td><li>하나의 객체를 생성하면 생성된 객체를 어디서든 참조할 수 있지만, 여러 프로세스가 동시에 참조할 수는 없다<li>클래스 내에서 인스턴스가 하나뿐임을 보장하며, 불필요한 메모리 낭비를 최소화할 수 있다</li></td></tr>
<tr>
<td>싱글톤<br>(Singleton)</td>
<td><li>하나의 객체를 생성하면 생성된 객체를 어디서든 참조할 수 있지만, 여러 프로세스가 동시에 참조할 수는 없다</li><li>클래스 내에서 인스턴스가 하나뿐임을 보장하며, 불필요한 메모리 낭비를 최소화할 수 있다</li></td>
</tr>
</table>

### 구조 패턴 (Structural Pattern)
- 구조가 복잡한 시스템을 개발하기 쉽도록 클래스나 객체들을 조합하여 더 큰 구조로 만드는 패턴
<table>
<tr>
<td>어댑터<br>(Adapter)</td>
<td><li>호환성이 없는 클래스들의 인터페이스를 다른 클래스가 이용할 수 없도록 변환해주는 패턴</li><li>기존의 클래스를 이용하고 싶지만, 인터페이스가 일치하지 않을 때 이용</li></td>
</tr>
<tr>
<td>브릿지<br>
(Bridge)</td>
<td><li>구현부에서 추상층을 분리하여, 서로가 독립적으로 확장할 수 있도록 구성한 패턴</li><li>기능과 구현을 2개의 별도 클래스로 구현</li></td>
</tr>
<tr>
<td>컴포지트<br>(Composite)</td>
<td><li>여러 객체를 가진 복합 객체와 단일 객체를 구분 없이 다루고자 할 때 사용하는 패턴</li><li>객체들을 트리 구조로 구성하여 디렉토리 안에 디렉토리가 있듯이 복합 객체 안에 복합 객체가 포함되는 구조를 구현 할 수 있다</li></td></tr>
<tr>
<td>데코레이터<br>
(Decorator)</td>
<td><li>객체 간의 결합을 통해 능동적으로 기능들을 확장할 수 있는 패턴</li><li>임의의 객체에 부가적인 기능을 추가하기 위해 다른 객체들을 덧붙이는 방식으로 구현</li></td></tr>
<tr>
<td>퍼사드<br>
(Facade)</td>
<td><li>복잡한 서브 클래스들을 피해 더 상위에 인터페이스를 구성함으로써 서브 클래스들의 기능을 간편하게 사용할 수 있도록 하는 패턴</li><li>서브 클래스들 사이의 통합 인터페이스를 제공하는 Wrapper 객체가 필요하다</li></td></tr>
<tr>
<td>플라이웨이트<br>
(Flyweight)</td>
<td><li>인스턴스가 필요할 때마다 매번 생성하는 것이 아니라, 가능한 공유해서 사용함으로써 메모리를 절약하는 패턴</li><li>다수의 유사 객체를 생성하거나 조작할 때 유용하게 사용할 수 있다</li></td></tr>
<tr>
<td>프록시<br>
(Proxy)</td>
<td><li>접근이 어려운 객체와 여기에 연결하려는 객체 사이에서 인터페이스 역할을 수행하는 패턴</li><li>네트워크 연결, 메모리의 대용량 객체로의 접근 등에 주로 이용</li></td></tr>
</table>


### 행위 패턴 (Behavioral Pattern)
- 구조가 복잡한 시스템을 개발하기 쉽도록 클래스나 객체들을 조합하여 더 큰 구조로 만드는 패턴
<table>
<tr>
<td>책임 연쇄<br>
(Chain of Responsibility)</td>
<td>
<li>요청을 처리할 수 있는 객체가 둘 이상 존재하여 한 객체가 처리하지 못하면 다음 객체로 넘어가는 형태의 패턴</li>
<li>요청을 처리할 수 있는 각 객체들이 고리(Chain)로 묶여 있어 요청이 해결될 때까지 고리를 따라 책임이 넘어간다</li>
</td>
</tr>
<tr>
<td>커맨드<br>
(Command)</td>
<td><li>요청을 객체의 형태로 캡슐화하여 재이용하거나 취소할 수 있도록 요청에 필요한 정보를 저장하거나 로그에 남기는 패턴</li><li>요청에 사용되는 각종 명령어들을 추상 클래스와 구체 클래스로 분리하여 단순화</li></td>
</tr>
<tr><td>인터프리터<br>(Interpreter)</td>
<td><li>언어에 문법 표현을 정희하는 패턴</li>
<li>SQL이나 통신 프로토콜과 같은 것을 개발할 때 사용</li></td>
</tr>
<tr>
<td>반복자<br>
(Iterator)</td>
<td><li>자료 구조와 같이 접근이 잦은 객체에 대해 동일한 인터페이스를 사용하도록 하는 패턴</li><li>내부 표현 방법의 노출 없이 순차적인 접근이 가능</li></td>
</tr>
<tr><td>중재자<br>(Mediator)</td>
<td><li>수많은 객체들 간 복잡한 상호작용(Interface)를 캡슐화하여 객체로 정의하는 패턴</li>
<li>객체 사이의 의존성을 줄여 결합도를 감소시킬 수 있다</li></td>
</tr>
<tr>
<td>메멘토<br>
(Memento)</td>
<td><li>특정 시점에서의 객체 내부 상태를 객체화함으로써 이후 요청에 따라 객체를 해당 시점의 상태로 돌릴 수 있는 기능을 제공하는 패턴</li>
<li>[Ctrl] + [Z]와 같은 되돌리기 기능을 개발할 때 주로 이용</li></td>
</tr>
<tr>
<td>옵저버<br>
(Observer)</td>
<td><li>한 객체의 상태가 변화하면 객체에 상속되어 있는 다른 객체들에게 변환된 상태를 전달하는 패턴</li>
<li>일대다의 의존성을 정의</li>
<li>주로 분산된 시스템 간 이벤트를 생성/발행(Publish)하고 이를 수신(Subscribe)해야 할 때 이용</li></td>
</tr>
<tr>
<td>상태<br>
(State)</td>
<td>
<li>객체의 상태에 따라 동일한 동작을 다르게 처리해야 할 때 사용하는 패턴</li>
<li>객체 상태를 캡슐화하고 이를 참조하는 방식으로 처리</li>
</td>
</tr>
<tr>
<td>전략<br>
(Strategy)</td>
<td><li>동일한 계열의 알고리즘들을 개별적으로 캡슐화하여 상호 교환할 수 있게 정의하는 패턴</li>
<li>클라이언트는 독립적으로 원하는 알고리즘을 선택하여 사용할 수 있으며, 클라이언트에 영향 없이 알고리즘 변경이 가능</li></td>
</tr>
<tr>
<td>템플릿 메소드<br>
(Template Method)</td>
<td>
<li>상위 클래스에서 골격을 정의하고, 하위 클래스에서 세부 처리를 구체화하는 구조의 패턴</li>
<li>유사한 서브 클래스를 묶어 공통된 내용을 상위 클래스에서 정의함으로써 코드의 양을 줄이고 유지보수를 용이하게 해준다</li></td>
</tr>
<tr>
<td>방문자<br>
(Visitor)</td>
<td><li>각 클래스들의 데이터 구조에서 처리 기능을 분리하여 별도의 클래스로 구성하는 패턴</li>
<li>분리된 처리 기능은 각 클래스를 방문(Visit)하여 수행</li></td>
</tr>
</table>

- 추상 클래스 (Abstract Class)
  - 구체 클래스에서 구현하려는 기능들의 공통점만을 모아 추상화한 클래스
  - 인스턴스 생성이 불가능하므로 구체 클래스가 추상 클래스를 상속받아 구체화한 후, 구체 클래스의 인스턴스를 생성하는 방식으로 사용
- 구체 클래스 (Concrete Class)
  - 인스턴스 생성이 가능한 일반적인 클래스를 의미하는 용어
  - 추상 클래스와 구분하기 위해 사용
  - 구상 클래스 또는 구현 클래스라고도 한다