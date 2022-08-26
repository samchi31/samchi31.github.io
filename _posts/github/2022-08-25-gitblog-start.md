---
layout: post
title: Git Blog 만들기
description: Git Blog 만드는 법 정리
categories: Github
tag: github
---

# Github를 이용해서 Blog를 만들기
## 1. jekyll을 이용하기 위해 ruby를 설치하고...할수도 있지만 원하는 테마를 골라 그 테마의 github 페이지를 fork하여 빠르게 테마를 적용할 수 있다.
  - jekyll 테마를 선택 한다. jekyll 테마를 모아둔 여러 사이트가 있다. 아래는 그 중에 내 맘에 드는 테마다. 
      - hydejack ( 모션? 이펙트?가 멋있다 )
        - hydejack을 쓰고 싶어서 ruby와 jekyll까지 설치했지만 로컬로만 접속되고 블로그 주소로는 접속이 되지 않았다. 
      - minimal-mistake ( 심플하다 )
      - NexT  ( 심플하면서도 모션이 어느정도 있다 내 블로그는 이 테마이다 )
  - 보통 download와 homepage(github 페이지) 방법이 있는데 둘 다 비슷하니까 더 간편한 homepage(github)에 들어가 fork 한다.  

## 2. 내 github에 들어가면 fork된 테마 repository를 볼 수 있다
  - repository의 이름을 'github이름.github.io'로 변경해준다.
    - repository의 setting의 page를 클릭해서 아래와 같이 뜬다면 주소를 입력해서 블로그에 바로 접속할 수 있다.
        ```
        Your site is live at 주소 
        ```
        
## 3. 바로 github 페이지에서 수정하거나 github repository를 로컬로 pull해서 수정해서 push한다.
  - _config.yml 을 수정한다.
    - title, url 등을 수정해본다.
    - github repository에서 Action을 눌러 적용이 완료됐는지 확인할 수 있다. 블로그 페이지를 새로고침해본다.
  - README.md, about/index.md 등을 수정해본다.

## 4. _posts 폴더 안에 포스트를 작성해본다.
  - _posts 폴더안에 폴더를 만들어 포스트들을 관리할 수 있다.  
    ```
    ---
    layout: post
    title: Git Blog 만들기
    description: Git Blog 만드는 법 정리
    date: 2022-08-25 00:00:00
    categories: 
    -github
    tag: 
    -github
    -test
    ---
    ```      
      - 파일 상단에 위처럼 작성한다. categories나 tag를 여러 개 사용할 수 있고 알아서 category가 생성된다.
      - 파일 제목은 YYYY-MM-DD-제목1-제목2.md 형식으로 작성하면 된다.
      - 테마에 기본적인 샘플 예시 페이지들이 작성되어있다. 참고해서 작성해본다.
        - 나는 블로그에 포스트가 안 떴었는데 위에서 date 부분을 삭제하니 포스트가 보였다.

## 5. assets/images 폴더 안에서 image를 바꿔본다.


#### ruby도 jekyll도 사용해 본 적이 없어서 테마 선택도 제한적이고 블로그 테마 선택도 제한적이였지만 카테고리별로 보기 쉬운 테마인 점을 생각하면 굉장히 만족스럽다.
