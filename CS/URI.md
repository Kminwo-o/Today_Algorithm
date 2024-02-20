## URI (Uniform Resource Identifier)
- Uniform : 리소스를 식별하는 통합된 방법
- Resource : 자원, URI로 식별할 수 있는 모든 것 (제한 없음)
- Identifier : 다른 항목과 구분하는데 필요한 정보 (ex : 주민등록번호)

### URI, URL, URN 어떤 차이가 있는가?
- URI
    - URI는 로케이터 (locator), 이름(name) 또는 둘 다 추가로 분류될 수 있다.
    - URL (Resource Locator) : 리소스의 위치를 의미, ex) Kminwo-o의 주소
    - URN (Resource Name) : 리소스의 이름 ex) Kminwo-o
- 즉, URL과 URN은 URI에 포함된 개념이다.
- URN은 중간에 어디 이름을 집어넣으면 매핑하는 것이 어려워 거의 URL만 쓴다.
- 이름은 변하지 않기 때문에 좋은 것 같지만 이름만으로 실제 리소스를 찾는 방법이 보편화되지 않아 잘 안쓰인다.

### URL 분석
- ex) https://www.google.com/search?q=hello&hi=ko
```plain
// 전체 문법
scheme://[userinfo@]host[:port][/path][?query][#fragment]

// 실제 문법
https://www.google.com:443/search?q=hello&hi=ko
```
- 스키마 : 주로 프로토콜 사용, 어떤 방식으로 자원에 접근할 것인가 하는 규칙
- http는 보통 80, https는 보통 443, 포트는 생략 가능
- userinfo@는 유저 정보를 포함하여 인증해야할 때 쓰나 거의 사용하지 않음.
