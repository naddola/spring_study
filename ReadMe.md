<H3>자바 코드로 직접 스프링 빈 등록하기</H3>
- 생성자를 통해서 들어오는 것이 생성자 주입(가장 좋은 주입)
- 필드에 @Autowired 하는 것이 필드 주입(바꾸기 힘들기 때문에 안좋은 방법)
- Setter를 통한 주입(public으로 작성해야하기 때문에 중간에 바뀔 위험이 있어서 안좋음)


- 실무에서는 주로 컴포넌트 스캔 방식을 사용함
- 정형화 되지 않거나, 상황에 따라 구현 클래스로 변경해야 하면 설정을 통해 스프링 빈으로 등록


- @Autowired를 통한 DI는 스프링이 관리하는 객체에서만 동작. 빈으로 등록하지 않으면 작동 하지 않음

<H2>회원 관리 예제 - 웹MVC 개발</H2>
<H3>회원 웹 기능 - 홈 화면 추가</H3>
- 요청이 들어오면 스프링컨테이너에 요청 주소가 있는지 확인하고 없으면 static으로 가게 되어있음. 
  localhost:8080으로 요청이 들어와도 "/"로 mapping이 되어있다면 index.html이 아닌 해당 컨트롤러로 가게 됨

<H3>회원 웹 기능 - 등록</H3>
<H3>회원 웹 기능 - 조회</H3>