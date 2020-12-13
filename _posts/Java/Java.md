---
title: "Java"
date: 2020-12-14 01:00:00 -0400
categories: Java
---

## ▶ Java
---
#### 1. Java (Java Programming Language)
썬 마이크로시스템즈(Sun Microsystems, Inc.)에서 공식적으로 발표한 객체지향 프로그래밍 언어이다. 현재는 오라클(Oracle)에서 썬을 인수했기에 오라클에 의해 배포되고 있다.

자바 코드를 실행하기 위해서는 JVM(자바 가상 머신, Java Virtual Machine)이라는 가상 머신이 필요한데, 이 가상 머신은 자바 바이트코드를 어느 플랫폼에서나 동일한 형태로 실행시킨다. 때문에 자바로 개발된 프로그램은 CPU나 운영 체제의 종류에 관계없이 JVM을 설치할 수 있는 시스템에서는 어디서나 실행할 수 있으며, 이 점이 웹 애플리케이션의 특성과 맞아떨어져 폭발적인 인기를 끌게 되었다.

#### 2. 자바의 특징
##### 운영체제에 독립적이다.
JVM의 위에서 작동하기 때문에 해당 운영체제에 적합한 JVM만 있으면 같은 코드로 여러 환경에서 실행시킬 수 있다.

##### 객체지향언어이다.
객체 지향 프로그래밍(Object-Oriented Programming, OOP)의 패러다임을 구현한 프로그래밍 언어이다.
객체 지향 프로그래밍이란 컴퓨터 프로그램을 명령어의 목록으로 보는 시각에서 벗어나 여러 개의 독립된 단위, 즉 "객체"들의 모임으로 파악하고자 한다.
그 주요한 특징에는 상속, 캡슐화, 다형성이 있다.

##### 가비지 컬렉터의 존재
가비지 컬렉터(Garbage Collector)가 자동적으로 메모리를 관리해주기 때문에, 프로그래머는 메모리를 따로 관리하지 않아도 된다.

##### 멀티쓰레드를 지원한다.
운영체제마다 구현방법과 처리 방식이 상이한 멀티쓰레드의 구현을 Java API를 통해 제공해준다.

##### 네트워크와 분산 처리를 지원한다.
TCP/IP 프로토콜, Http 프로토콜 등 다양한 네트워크 프로그래밍 라이브러리를 통해 비교적 짧은 시간에 네트워크 관련 프로그램을 쉽게 개발할 수 있도록 지원한다.

##### 동적 로딩을 지원한다.
실행시가 아닌 필요한 시점에 클래스의 로딩이 가능하다.

##### 함수형 프로그래밍
JDK 1.8에서 추가된 Lambda식과 함수형 인터페이스를 활용하면 함수형 프로그래밍 또한 가능하다.

#### 3. 자바 플랫폼
자바의 개발 환경과 실행 환경을 제공한다. Java SE, Java EE, Java ME가 있다.

##### Java SE
Java SE(Java Platform, Standard Edition)는 표준 자바 플랫폼으로 표준적인 컴퓨팅 환경을 지원하기 위한 표준적인 JVM의 규격 및 API 집합을 포함하고 있는 플랫폼이다.

##### Java EE
Java EE(Java Platform, Enterprise Edition)은 자바를 이용한 서버측 개발을 위한 플랫폼이다. Java SE에 부가하여, 웹 애플리케이션 프로그래밍에서 사용하는 JSP, Servlet, JDBC, 장애복구 및 분산 멀티티어 등 기능이 추가되어 있다.

##### Java ME
Java ME(Java Platform, Micro Edition)은 제한된 자원을 가진 휴대 전화, PDA, 세트톱박스 등에서 Java 프로그래밍 언어를 지원하기 위해 만들어진 플랫폼을 가리킨다. 스마트폰으로 바뀌면서 요즘엔 잘 쓰이지 않는다.

#### ▶ Reference
- https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94_(%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D_%EC%96%B8%EC%96%B4)
- 남궁성, 『자바의 정석』, 도우출판
- <a href="https://blog.naver.com/PostView.nhn?blogId=rorean&logNo=221636124268&categoryNo=16&parentCategoryNo=0&viewDate=&currentPage=1&postListTopCurrentPage=1&from=postView
">[java] Java SE, Java EE, Java ME 차이</a>
