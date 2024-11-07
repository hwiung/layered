대부분의 구조가 '정형화' 돼 있는 메모 CRUD API를 만들었으며, 이제 실습을 기반으로 모든 CRUD API를 만들 수 있게 됐다. -> 정형화 돼 있으니깐, 실습으로 만든 메모 API를 응용하여 다른 형태로 만들면 된다.

해결한 문제점
  1. 데이터베이스에 영구적으로 테이터가 저장되지 않는 것(DataBase 접근 기술).

유효한 문제점
  1. 예외 발생시 공통적으로 처리가 불가능하다.
       각각의 모든 예외를 try-catch 해서 처리해야 한다.
  2. RequestDto, ResponseDto를 공유하여 null 값이 들어 오기도 한다.
       필요 없는 필드에 추가적인 null 검사를 해야한다.
  3. Spring Bean, 생성자 주입 등 Spring의 동작 원리에 대해 이해하지 못했다.
  4. 왜 Interface로 만들어서 구현하여 사용하는지 모른다.

중요한 점
 1. Client to Server 데이터 전송하는 방법 3가지
    - GET + Query Parameter(=Query String)
    - POST + HTML Form(x-www-form-urlencoded)
    - HTTP Request Body

 2. erver to Client 데이터 응답하는 방법 3가지
    - 정적 리소스
    - View Template
    - HTTP Response Body
