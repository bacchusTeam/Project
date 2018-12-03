---
layout: post
title: New Project 1
date: 2018-11-28 13:00:00
categories: TIL
tag: Gradle, Eclipse
---
# New Project 1

git submodule 이용한 다중 repo 프로젝트 1개만 이용한 mono repo 프로젝트  

|repo 개수|장점|단점|
|:---|:---:|---:|
|mono (1)|구성의 단순함|프로젝트가 커지면 복잡해짐|
|multi (복수)|repo 별 독립성 보장 다중 프로젝트 진행시 유용|git 관리 복잡|

프로젝트간에 독립성이 어느 정도 보장되는것이 핵심이면 multi 가 좋을거 같고  
규모가 좀 작으며서 쉽게 시작 하기는 mono 가 좋을거 같음 그래서 mono 로 ㄱㄳ

## 1. Gradle Multi Module with Eclipse

Gradle 이용한 Multi Module 설정하기
[예제](https://github.com/deuxksy/java-skeleton/tree/master/spring-boot-multi-module)

## 2. Gradle 5 가 나와서 다시 공부 하면서 다시

[예제](https://github.com/deuxksy/TIL/tree/master/Gradle/gradle-multi-project)