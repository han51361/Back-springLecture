## 백기선님의 예제로 배우는 스프링 입문 강좌

### Spring PetClinic Sample Application [![Build Status](https://travis-ci.org/spring-projects/spring-petclinic.png?branch=main)](https://travis-ci.org/spring-projects/spring-petclinic/)

##### Understanding the Spring Petclinic application with a few diagrams
<a href="https://speakerdeck.com/michaelisvy/spring-petclinic-sample-application">See the presentation here</a>

## Running petclinic locally
Petclinic is a [Spring Boot](https://spring.io/guides/gs/spring-boot) application built using [Maven](https://spring.io/guides/gs/maven/). You can build a jar file and run it from the command line:


# 8강. DI(Dependency Injection)
-필요한 의존성을 어떻게 받아올 것인가. 

**@Autowired / @Inject를 어디에 붙일까**

**생성자(권장)**
:` 필수적으로 사용해야하는 레퍼런스없이는 인스턴스를 만들지 못하도록 강제할 수 있기 떄문에`
* 필드
* Setter
`(예외 : 순환참조 - A와 B가 서로 참조시에 생성자 Injection 사용으 만들지 못한다.
따라서 필드 or Setter Injection 을 사용해야한다. )`
- 과제 : 
 ownerController에 petRepository  주입하기 
