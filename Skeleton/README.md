# Spring 5 에 대해 알아보자

Sample 은 아래 2곳 만을 참조 해서 사용하자

- [Spring Framework Guide](https://spring.io/guides)
- [Spring Boot Sample](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples)

## complete 비즈니스 로직이 들어가지 않은 단순 뼉따구

4개의 multi project 가 목표

### spring-boot-skeleton-core

util, web, batch 모두 사용되는 core

### spring-boot-skeleton-util

web, util 에서 사용되는 단순 util

### spring-boot-skeleton-web

web

### spring-boot-skeleton-batch

batch

## initial 단순 참조 예제

sample 예제의 원문을 참조 하고 싶으면 git 을 확인 실제 하위 폴더 에 있는 파일들은 수정돤 소스들 아닐수도 있음 ㅋ

```bash
  git config --system core.longpaths true # windows 에서 파일명이 길때 발생함
```

### mvn 구동 방법

```bash
  mvn spring-boot:run # spring boot 실행 하기
  mvn clean compile # 삭제 및 컴파일
  mvn test # 테스트
```

### [spring-boot-sample-simple](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-simple)

banner.txt 는 알았지만 banner.jpg 도 된다 2.0 에서 추가 된건가 ㅋ 참신해  
banner.txt 만들어 주는 [사이트](https://devops.datenkollektiv.de/banner.txt/index.html)  
banner.txt 에서 [사용가능 한 변수](https://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-spring-application.html#boot-features-banner)

### [spring-boot-sample-logback](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-logback)

아주 간단한 spring boot 와 logback 이용해서 단순 로그를 남기는 예제 추가 가능 하다면 lombok 도 사용해보자

### [spring-boot-sample-web-jsp](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-web-jsp)

jsp controller 연결하는 아주 간단한 웹 예제

### [spring-boot-sample-tomcat](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-tomcat)

spring mvc 를 이용한 간단한 웹

### [spring-boot-sample-flyway](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-flyway)

flyway(db migration tool) 와 h2(in memory db) 이용한 예제

### [spring-boot-sample-web-secure](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-web-secure)

security 이용한 단순한 로그인 application.yml 계정정보를 가지고 로그인 하는 예제