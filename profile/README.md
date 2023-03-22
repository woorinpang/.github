## [키트 주문 제작소] 👋

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

<!-- ## Client Server
| 서버 | 설명 |
| --- | --- |
| [JEEOK-CLIENT-VUE](https://github.com/heechul90/project-jeeok/tree/main/jeeok-client-vue) | Front end 서버 |

## API Gateway Server
| 서버 | 설명 |
| --- | --- |
| [APIGATEWAY-SERVER](https://github.com/heechul90/project-jeeok/tree/main/apigateway-server) | 모든 요청을 통과하는 API 라우팅 서버 |

## Config Server
| 서버 | 설명 |
| --- | --- |
| [CONFIG-SERVER](https://github.com/heechul90/project-jeeok/tree/main/config-server) | 각 서버의 application.yml을 관리하는 서버 |
-->

## Config
| 서버 | 설명 |
| --- | --- |
| [CONFIG-SERVER]() | 설정 |
| [DISCOVERY-SERVER]() | 유레카 서버 |
| [APIGATEWAY]() | api 게이트웨이 |


## Service
| 서비스 | 설명 |
| --- | --- |
| [USER-SERVICE]() | 사용자 서비스 |
| [STORE-SERVICE]() | 스토어 서비스 |
| [ORDER-SERVICE]() | 주문 서비스 |
| [DELIVERY-SERVICE]() | 알림 서비스 |
| [NOTIFICATION-SERVICE]() | 알림 서비스 | 


## 사용 기술스텍
| 기술스택 | 개발환경 |
| --- | --- |
| Spring | - String Boot 3.0.x </br> - Java 17 </br> - Gradle </br> - Spring Web Mvc </br> - Spring Security |
| Spring Cloud | - Eureka </br> - Gateway </br> - Config </br> - OpenFeign |
| Authenticate | - JWT (Json Web Token) |
| ORM | - JPA </br> - Querydsl |
| Database | - MariaDB </br> - Redis |
| Test | - Spring RestDocs </br> - JUnit5 </br> - Mock |
| Message Queue | - Kafka |
| Monitoring | - Spring Cloud Sleuth </br> - Zipkin |

## 시스템 아키텍처

## 브랜치 전략
- main
  - hot-fix
- develop
  - feature
  - refactor

## 테스트 전략
테스트는 통합테스트(Integration), 단위테스트(Mock), 레포지토리테스트(DataJpaTest)로 나우어 진행한다.
- controller : 통합테스트, 모든 bean을 올리고 운영환경과 가장 유사하게 테스트를 한다.
- service : 단위테스트, 진행하고자 하는 테스트에만 집중하여 테스트한다.
- repository : 레포지토리테스트, 관련된 Bean들만 등록하여 통합테스트 보다 빠르게 테스트를 진행한다.
  
  
