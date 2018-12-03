# Spring 5 에 대해 알아보자

Sample 은 아래 2곳 만을 참조 해서 사용하자

- [Spring Framework Guide](https://spring.io/guides)
- [Spring Boot Sample](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples)

## 1. spring-boot-skeleton

비즈니스 로직이 들어가지 않은 단순 뼉따구 4개의 multi project 가 목표  

### 1.1. spring-boot-skeleton-core

util, web, batch 모두 사용되는 core

### 1.2. spring-boot-skeleton-util

web, util 에서 사용되는 단순 util

### 1.3. spring-boot-skeleton-web

web

### 1.4. spring-boot-skeleton-batch

batch

## 2. spring-boot-sample

Maven 기반을 gradle 구동이 가능 하게 설정 원문을 참조 하고 싶으면 [Spring Boot Sample](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples) 확인

git 사용중 windows 파일명 길어서 git 오류 발생시 처리

```bash
  git config --system core.longpaths true # windows 에서 파일명이 길때 발생함
```

### 2.1. mvn 구동 방법

spring-boot-sample-tomcat 은 gradle 변환 하지 않음 손이 좀 많이 감 mavne 직접 테스트

```bash
  mvn spring-boot:run # spring boot 실행 하기
  mvn clean compile # 삭제 및 컴파일
  mvn test # 테스트
```

### 2.2. [spring-boot-sample-simple](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-simple)

banner.txt 는 알았지만 banner.jpg 도 된다 2.0 에서 추가 된건가 ㅋ 참신해  
banner.txt 만들어 주는 [사이트](https://devops.datenkollektiv.de/banner.txt/index.html)  
banner.txt 에서 [사용가능 한 변수](https://docs.spring.io/spring-boot/docs/current/reference/html/boot-features-spring-application.html#boot-features-banner)

### 2.3. [spring-boot-sample-logback](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-logback)

아주 간단한 spring boot 와 logback 이용해서 단순 로그를 남기는 예제 추가 가능 하다면 lombok 도 사용해보자

### 2.4. [spring-boot-sample-web-jsp](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-web-jsp)

jsp controller 연결하는 아주 간단한 웹 예제

### 2.5. [spring-boot-sample-tomcat](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-tomcat)

spring mvc 를 이용한 간단한 웹

### 2.6. [spring-boot-sample-flyway](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-flyway)

flyway(db migration tool) 와 h2(in memory db) 이용한 예제

### 2.7. [spring-boot-sample-web-secure](https://github.com/spring-projects/spring-boot/tree/master/spring-boot-samples/spring-boot-sample-web-secure)

security 이용한 단순한 로그인 application.yml 계정정보를 가지고 로그인 하는 예제