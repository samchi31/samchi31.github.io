---
layout: post
title: 객체지향프로그래밍 3요소 5원칙
description: 객체지향프로그래밍 3요소 5원칙 정리
categories: Java
tags: java
---

# 객체지향프로그래밍 3요소
- 캡슐화(Encapsulation)  
  - 정보 은닉. 
  - 같은 기능을 목적으로 하는 코드들을 한 클래스로 모으고 클래스 내부의 필드는 private로 선언하고 메서드는 public으로 작성하여 객체 간 결합도를 낮출 수 있다.
- 상속(Inheritance) 
  - 자식 클래스가 부모 클래스를 상속받아 부모의 클래스 멤버에 접근할 수 있다.
- 다형성(Polymorphism) 
  - 하나의 객체가 여러가지 형태로 바뀔 수 있는 것이다. 
  - 메서드 오버라이딩(Overriding)을 하여 부모에서 상속받아 자식기능을 확장할 수 있다. 
  - 오버로딩(Overloading)으로 같은 메서드의 이름으로 다양한 매개변수로 동작하게 할 수 있다.

# 객체지향프로그래밍 5원칙 (SOLID)
- 단일 책임 원칙(Single Responsibility Principle)
  - 클래스는 단 한개의 기능을 가져야 한다.
- 개방-폐쇄 원칙(Open Closed Principle)
  - 클래스는 확장에 열려(Open)있어야 하고 수정에는 닫혀(Close)있어야 한다.
- 리스코프 치환 원칙(Liskov Substitution Principle)
  - 자식 클래스는 언제나 부모 클래스를 대체할 수 있어야 한다.
  - 부모 클래스와 자식 클래스 사이의 기능이 일관성이 있어야 한다.
- 인터페이스 분리 원칙(Interface Segregation Principle)
  - 한 클래스는 자신이 사용하지 않는 인터페이스는 구현하지 말아야 한다.
  - 클라이언트에 맞게 인터페이스가 구현되어야 한다.
- 의존 관계 역전 원칙(Dependency Inversion Principle)
  - 고차원 모듈은 저차원 모듈에 의존하면 안 된다. 
  - 추상화된 것은 구체적인 것에 의존하면 안 된다.
  - 구체적인 것이 추상화 된것에 의존해야 한다.
