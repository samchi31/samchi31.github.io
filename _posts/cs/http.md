# request packaging 규칙

# request 객체 part
- request line : 받는 사람 주소 (URI, method )
- request header : 메타데이터가 들어감 (있어도 되고 없어도 되고 필수 아님)
- request body : (필수 아님) 요청을 보내는 목적에 따라

## request header
1. client가 수용할 수 있는 데이터 (응답데이터 헤더와 일치) - 중요!accept로 시작하는 ~ 
- accept: client가 받아들이는 정보 타입
- accept-encoding : 압축
- accept-language : locale code (언어-지역)

2. client의 정보를 부가적으로 세팅할 데이터
- cache-control : cache 사용 여부, jsp 서블릿에서는 기본적으로 no-cache
- connection : http 3-hand-shaking으로 최초 연결, http는 원래 한번 요청 후 연결끊음(connectless) 비효율적이어서 keep-alive(connection 재활용)
- cookie : 클라이언트 쪽에 저장됨 서버쪽으로 동일한 데이터가 재전송 서버에서 생성 (Session Tracking Mode) 
- user-agent : client의 접근 환경 정보 (desktop, mobile

# 표준 메서드
- get, post


## classpath resource, filesystem resource,

## classLoader => classpath 관리자
