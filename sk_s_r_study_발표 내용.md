---
tags:
  - SK_shieldus_rookes
---

HTML

	1. HTML5 새로운 입력타입으로 추가된 것
		 email,url,number,range,Data pickers,search,color
		 
	2. HTML입력필드 생성요소
	3. HTML5 세션 스토리지와 로컬스토리지를 다루는 객체
		web storage object
		
	4. HTML5새로운 시맨틱요소
		header,nav,main,section,article,figure & figcaption,footer 

CSS

	1. 특정 클래스 이름을 가진 요소를 선택하는 CSS선택자
		CSS 기본 문법: 선택자 { 속성1: 값1; 속성2: 값2; ... }
			클래스 선택자: .클래스명{```}
				        .클래스명.클래스명{```}
	2. CSS요소 위치제어 속성?
		static
			기본적으로 설정되는 값으로, 요소를 문서의 흐름에 맞추어 배치합니다. 
			다른 위치 속성들과 달리 추가 속성을 사용하지 않습니다.
		relative
			이전 요소에 자연스럽게 연결하여 배치하되 상대적인 위치를 지정할 수 있습니다. 
			top, right, bottom, left 속성을 사용하여 요소를 이동시킬 수 있습니다.
		absolute
			요소를 문서 흐름에서 제거하고,가장 가까운 위치 지정 조상 요소에 상대적으로 
			배치합니다. 
			위치 지정 조상이 없을 경우에는 문서의 초기 컨테이너를 기준으로 배치됩니다.
		fixed
			요소를 뷰포트에 상대적으로 배치합니다. 
			스크롤되더라도 화면의 고정 위치에 요소가 표시됩니다.
		sticky
			요소가 스크롤되는 영역에 따라 상대적인 위치를 변경합니다. 
			스크롤 영역을 벗어나지 않는 한 일정 위치에 고정됩니다.
			
	3. 자식요소를 선택하는 CSS 선택자
		선택자 { 속성1: 값1; 속성2: 값2; ... }
		자식 선택자:   선택자1 선택자2{```}
					선택자1 > 선택자2{```}
					
	4. CSS주요역할
		브라우저에서 HTML 요소의 모양을 정확하게 제어하고 원하는 디자인을 사용하여 
		마크 업을 표시

JavaScript , ES6 , TSX

	1. ES6 함수의 기본 매개변수 값 설정방법
		function multiply(a, b = 1) {
		  return a * b;
		}
		
		console.log(multiply(5, 2));
		// Expected output: 10
		
		console.log(multiply(5));
		// Expected output: 5
		
	2. JavaScript 비동기 처리에 사용하는 객체
		Promise
			비동기 작업의 성공 또는 실패에 대한 결과를 나타내는 객체
			처음에는 Pending(대기)상태, 
			작업이 성공적으로 완료되면 Fulfilled(이행)상태, 
			실패하면 Rejected(거부)상태가 된다.
			
	3. ES6 새로운 변수선언 키워드는?
		let 키워드(블록스코프) 
		선언되면, 선언과 초기화가 분리되어 이뤄지며, 블록스코프를 가지며 선언된다. 
		나아가 let은 변수의 값을 재할당하여 변경할 수 있지만, 기존의 var가 가지고 있던 한계가
		 극복되어, 같은 이름으로 변수를 재선언하는 것은 불가능하다는 것이며, 
		 이를 통해서 코드의 안정성이 높아지게 되었다.
		
		const 키워드(블록스코프)
			선언과 함께 값을 할당해야 한다. 
			즉 재할당이 불가능한 키워드가 const 인데, 이러한 특징으로 상수라고 불리기도 
			한다. 
			그럼에도 해당 키워드로 선언된 식별자가 객체나 배열을 대입받고 있다면 메모지에 
			저장되는 특징으로 그 내의 값이 변경될 수 있기도 하다. 
			그러기에 완전한 상수라고 부를 수는 없다.
			
	4. TSX?
		TS와 TSX의 차이
		TS (TypeScript)
			TypeScript는 JavaScript를 기반으로 하며, 정적 타입 검사를 지원하는 
			JavaScript의 슈퍼셋이다. TS는 대개 .ts 파일 확장자를 사용한다.
		TSX (TypeScript with JSX)
			TSX는 React에서 UI를 작성하는 데 사용되는 TypeScript이다. 
			React에서 JSX를 사용하는 경우 일반적으로 TSX 파일 확장자를 사용한다.
		
		따라서, TS는 JavaScript 코드에서 타입 검사와 컴파일 타임 오류 검사를 수행하는 데 
		사용되고, TSX는 React에서 UI를 작성할 때 TypeScript를 사용하여 타입 검사를 수행
		하는 데 사용된다.
		
	5. ES6 추가된 화살표 함수 사용예시
		const materials = ['Hydrogen', 'Helium', 'Lithium', 'Beryllium'];
		console.log(materials.map((material) => material.length));
		// Expected output: Array [8, 6, 7, 9]
		
	6. JavaScript 프레임워크
		Ember,Angular,Vue,React 등
		
	7. JavaScript의 용도
		동적으로 변경되는 콘텐츠를 만들고, 멀티미디어를 제어하고, 이미지에 애니메이션을 적용
		하는 등 거의 모든 작업을 수행할 수 있는 스크립팅 언어
		
	8. ES6문자열 템플릿리터럴 사용방법
		문자역을 작성할 때 백틱(`)을 이용해서 작성한 뒤 변수를 삽입하고 싶은 부분에 ${}를
		 사용해 변수를 넣어주면 된다.
			let name = "yeri"
			consol.log('hi i am $(name)')
			//output : hi i am yeri
	

리액트

	1. 리액트 컴포넌트간 데이터 전달방법
		
		부모컴포넌트->자식컴포넌트
			1. props통째로 넘기기
				const Parent = () => {
				  const data1 = 100;
				  const data2 = 200;
				  return (
				    <div>
				      <Child 
				    	data1={data1}
						data2={data2}
					  />
				    </div>
				const Child = (props) => {
				  return (
				    <p>{props.data1}</p>
				    <p>{props.data2}</p>
				  );
				};
			2.비구조화 할당으로 하나씩 넘기기
				const Parent = () => {
				  const data1 = 100;
				  const data2 = 200;
				  return (
				    <div>
				      <Child 
				    	data1={data1}
						data2={data2}
					  />
				    </div>
				const Child = ({ data1, data2 }) => {
				  return (
				    <p>{data1}</p>
				    <p>{data2}</p>
				  );
				};
		자식컴포넌트->부모컴포넌트
			함수 포인터를 넘기면 부모 컴포넌트에 데이터를 전달할 수 있다.
			1. 부모에 상태를 업데이트 하는 함수를 만든다.
			2. 자식에게 해당 함수를 가리키는 포인터를 props로 넘긴다.
			3. 자식 컴포넌트는 props로 받은 함수의 파라미터로 데이터를 넘긴다.
			4. 부모 컴포넌트에게 전달 완료

	2. 리액트의 상태(state) 변경함수
		<div 이벤트={()=>{변경함수(변경내용)}}></div>
		
	3. 리액트 생명주기 메서드
		생명주기는 크게 maunting,update,unmaunting으로 나눌수있다.
		
		마운트시 호출되는 메서드
			1. constructor: 컴포넌트를 새로 만들 때마다 호출되는&nbsp;클래스 생성사 메서드
			2. getDerivedStateFromProps:&nbsp;props&nbsp;에 있는 값을
									   &nbsp;state&nbsp;에 넣을 때 사용하는 메서드
			1. render: 준비한 UI를&nbsp;렌더링하는 메서드
			2. componentDidMount:&nbsp;컴포넌트가 웹 브라우저상에 나타난 후 호출하는 메서드
		
		업데이트에 호출되는 메서드
			1. getDerivedStateFromProps: 앞서&nbsp;Mount&nbsp;과정에서도 호출되고,
					&nbsp;props 변화에 따라 state&nbsp;값에도 변화를 주고 싶을 때 사용
			2. shouldComponentUpdate:&nbsp;컴포넌트가 &nbsp;리렌더링을 해야 할지 말아야
										할지를 결정,&nbsp;true를 반환하면 &nbsp;
										다음 라이프사이클 메서드를 계속 실행,
										&nbsp;false&nbsp;를 반환하면 
										&nbsp;작업을 중지(리렌더링 X)한다.
			1. render: 컴포넌트를&nbsp;리렌더링한다.
			2. getSnapshotBeforeUpdate: 컴포넌트 변화를 DOM에 반영하기 바로 직전에 호출
			3. componentDidUpdate:&nbsp;컴포넌트의 업데이트 작업이 다 끝난 후 호출
		
		언마운트시 호출하는 메서드
			1. componentWillUnmount:&nbsp; 컴포넌트가 웹 브라우저상에서 사라지기 전에
								   호출
	1. 리액트 Context ADI사용하는 목적
		Context ADI 는 상태 관리를 위해 사용
			상태 관리의 목적은 애플리케이션의 상태를 효율적으로 관리하여, 
			코드의 가독성을 높이고 유지 보수를 용이하게 하는 것입니다.
				작은 규모의 프로젝트나 간단한 상태 공유가 필요한 경우, 
				Context API의 간결함과 리액트 내부 기능을 활용한 접근 방식이 더 적합할 수 있습니다.

Java , spring

	1. Java객체생성 문법
![[Pasted image 20240715231955.png]]

	2. 스프링 빈(bean) 정의한 애노테이션
		XML <bean/> 구성 요소와 유사하다. 이것은 스프링 빈을 만들고 일반적으로&nbsp;_@Configuration_과 함께 사용된다. 
		우리는 메소드 수준에서 *@Bean_을 사용한다. 
		앞서 언급한&nbsp;_@Configuration_이 있는 클래스(구성 클래스라고 부른다)는 객체를 초기화하는 메소드를 가지고 의존 관계를 구성한다. 
		그런 메소드는 *@Bean_&nbsp;어노테이션을 가지게 될 것이다. 
		기본적으로, 빈 이름은 메소드 이름과 동일하다. 
		초기화한 다음 실제 빈을 리턴한다. 
		그 어노테이션이 있는 메소드는 스프링 IoC 컨테이너에서 관리되는 빈을 만들게 된다.
		
	3. Spring 의존성 주입을 구현하기 위해 사용된 개념
		&nbsp;@Autowired 어노테이션을 사용하여 의존성 주입을 손쉽게 구현
		
	4. Java주석 처리방법
		한 줄만 주석처리 ( // ), 여러 줄을 주석 처리 (/* */), 문서화 주석 (/** */)
		단축키는 ctrl + / 
		
	5. SpringBoot RESTful 웹서비스 개발 어노테이션
		@RestController 를 사용하여 RESTful API 를 작성
		
	6. Java 기본 데이터타입
		byte, short, int, long,float, double,boolean,char
			내용정리 내 표
			
	7. Spring 프레임 워크의 주요모듈
![[Pasted image 20240716144622.png]]

DB

	1. DB 데이터 검색하기위해서 사용하는 언어
		SQL(DML)
		
	2. DB정규화목적
		1. 불필요한 데이터를 제거해 불필요한 중복을 최소화
		2. 데이터베이스 구조 확장시 재디자인을 최소화
		3. 다양한 관점에서의 Query를 지원
		4. 무결성 제약조건의 시행을 간단하게
		5. 각종 이상 현상(Anomaly)을 방지
		6. 테이블의 구성을 논리적이고 직관적으로 구성
		
	3. DB 기본키 목적
		데이터베이스 테이블의 모든 레코드를 식별하는 것
		
	4. SQL DB 트랜젝션의 특성을 나타내는 약어
		ACID
			원자성(Atomicity), 일관성(Consistency), 격리(Isolation), 영속성(Durability)
			

마이크로 서비스

	1. 마이크로 서비스 아크턱 서비스가 독립적으로 개발,배포,운영을 지원하는 도구
		Doker,Kubernetes
		
	2. 마이크로 서비스 트랙잭션을 관리하기위해 사용되는 (...?)
		Saga Pattern
	3. 마이크로 서비스 각 서비스의 통신방법
		동기적 Synchronous&nbsp;통신 방식과 비동기적Asynchronous 메시지 전달 방식
		
		동기적 통신
			HTTP나 RPC 같은 프로토콜을 이용하여 다른 서비스가 노출한 API를 호출하는 방식입니다. 
			호출자가 답변을 기다리기 때문에 동기적 메시징 패턴입니다.
		비동기적 메시지 전달 방식
			서비스에서 메시지를 보낸 뒤 답변을 기다리지 않는 방식입니다. 
			하나 혹은 다수의 서비스가 메시지를 비동기적으로 처리합니다.
			
	4. 마이크로 서비스의 장점
		1. 각 서비스가 독립적으로 배포되고 운영되기 때문에, 서비스 간의 의존성을 줄일 수 있습니다.
		2. 각 서비스가 독립적으로 개발되기 때문에, 개발 속도를 높일 수 있습니다.
		3. 각 서비스가 독립적으로 확장될 수 있기 때문에, 시스템의 확장성을 높일 수 있습니다.

REST API

	1. REST API 서버로 클라이언크로 전송되는 데이터의 미디어 타입을 지정하시위해 사용하는 HTTP 헤더는?
		표현 헤더(Representation&nbsp;Headers)
		
	2. REST API 데이터를 가져오는 HTTP메서드
		GET
		
	3. REST API 엔드포인트 설계시 리소스를 표현하는 방식
		` https://mysite.com/posts `
		
	4. REST API 특징
		Server-Client 구조
		Stateless
			HTTP 프로토콜은 Stateless Protocol 이므로 REST 역시 무상태성을 갖는다.
			 Client의 context를 Server에 저장하지 않는다.  
		Server는 각각의 요청을 완전히 별개의 것으로 인식하고 처리한다.
		Cacheable
			Http의 특징인 캐싱 기능을 적용할 수 있다. 캐시 사용을 통해 응답 시간이 빨라진다.
		Layered System
			Client는 REST API Server만 호출하고, REST Server는 다중 계층으로 구성될 수 있다.
		Uniform Interface
			URI로 지정한 Resource에 대한 조작을 통일되고 한정적인 인터페이스로 수행한다.
		Self-descriptiveness
			REST API 메세지만 보고도 이를 쉽게 이해할 수 있는 자체 표현 구조로 되어있다.
			
	5. REST 주요 원칙 중 자원을 고유하게 식별하기 위해 사용하는것
		RESTful API 설계 원칙
			모든 자원은 고유한 URI를 가지며, 이를 통해 자원을 식별합니다.

