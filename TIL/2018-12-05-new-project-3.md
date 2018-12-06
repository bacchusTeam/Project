---
layout: post
title: New Project 2
date: 2018-12-05 10:00:00
categories: TIL
tag: Spring, Boot, Application.yml
---
# New Project 2

off 스터디 3일차

## 1. Spring Boot Web

[Spring Guides](https://github.com/spring-guides) 예제 들은 프로젝트 만들기 조금 애매한  
간다한 팁 이라면 clone 하고 root 폴더에 settings.gradle 파일을 만들고 eclipse 에서 gradle 프로젝트로 읽기
```groovy
rootProject.name=gs-rest-service
include ('complete')
include ('initial')
```

### 1.1 [간단한 rest api 구축](https://github.com/spring-guides/gs-rest-service)

reset api 만들어 보자

### 1.2 [간단한 mvc](https://github.com/spring-guides/gs-serving-web-content)

static index.hthml 이용한 접속 및 mvc 이용한 greeting.html 접속
간단한 devtools 예제 해보기

### 1.3 Spring Boot > Spring Starter Project 만들어 보기

- devtools
  - buildg.radle runtimeOnly('org.springframework.boot:spring-boot-devtools')
  - [chrome plugin](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei)
  - [idea option](http://haviyj.tistory.com/11)

## 2. Application.yml

[application.yml](https://docs.spring.io/spring-boot/docs/current/reference/html/common-application-properties.html) 원본 문서 모든 값을 확인 해보고

### 2.1 [so-yaml](https://github.com/konrad-garus/so-yaml)

예제로 해보자

```java
@Value("${hello}")
private String hello;

@Value("${ksy.name}")
private String name;

@Value("${ksy.friend}")
private String[] friend;

@Autowired
AvailableChannelsConfiguration availableChannelsConfiguration;
```

```yml
hello: 어서와

ksy:
  name: 김석영
  friend: 김욱진,양주환

availableChannelsConfiguration:
 ...
 ...
 ...

```

- 단순 출력
- List 형태 출력
- @Configuration 형태 출력
