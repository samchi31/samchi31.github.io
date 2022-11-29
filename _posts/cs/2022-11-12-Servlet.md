---
layout: post
title: 서블릿
description: 서블릿 정리
categories: cs
tags: 
- java
- cs
- servlet
---

# 서블릿 (Servlet)
- Web Application에서 Client의 요청(request)을 처리하고 응답(response)을 Client에게 전송
- init() : 서블릿 객체 초기화
- service() : request들이 들어오면 웹 컨테이너가 service()를 호출해 request들을 스레드에서 처리
- destory() : 서블릿 객체 파괴 자원 release


# 서블릿 컨테이너 (Servlet Container)

## 웹서버(Web Server)
- 웹서버 : 웹페이지를 사용자에게 전송하는 서버. 

## 서블릿 컨테이너
- 서블릿을 관리 : 서블릿들의 생성, 실행, 파괴를 담당
- 서블릿들을 위한 상자(Container)
- 웹 서버와 소켓을 만들어 통신
- 톰캣이 대표적인 예시

# 서블릿 컨텍스트 (Servlet Context)
- HTTP 프로토콜 통신 방식은 비연결형 통신 방식, 즉 Client로부터 응답을 하면 연결이 끊어지고 요청이 있을 때마다 새롭게 연결한다.
- 클라이언트 정보 유지가 안됨 -> Servlet Context를 이용

## 서블릿 컨텍스트
- 하나의 서블릿이 서블릿 컨테이너와 통신하기 위해서 사용되는 메소드를 지원하는 인터페이스
- 웹 어플리케이션 단위로 하나의 Servlet Context 객체가 생성
