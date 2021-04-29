---
layout: post
title: 안드로이드 인터뷰정리
subtitle: android 면접
tags: [android,interview,안드로이드,면접 ]
published: false
---

# 자바 질문 정리
## 오버로딩과 오버라이딩의 차이
### -오버로딩
    같은 이름에 메소드를 여러개 정의하고 각 파라미터의 타입과 갯수를 다르게하여 표현할수 있는 기술
### -오버라이딩
    상위 클래스,인터페이스로 부터 함수를 상속받아 재정의함



# Android 면접 정리

## Context 가 무엇인가?
### [참고링크](https://shinjekim.github.io/android/2019/11/01/Android-context%EB%9E%80/) 
    안드로이드 4대 컴포넌트의 추상 클래스로 
    Context-ContextWrapper-(Activity,Service,...)으로 구성되어있다.
    Context 는 Application 내의 시스템이 관리하는 정보에 접근할 수 있는것.
    -Application Context
    앱 생명주기에 맞춰져있는 context
    -Activity Context
    액티비티 생명주기에 맞춰져있는 context
    
## 안드로이드 4대 컴포넌트 설명
### [참고링크](https://velog.io/@jojo_devstory/%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C-Android-4%EB%8C%80-%EC%BB%B4%ED%8F%AC%EB%84%8C%ED%8A%B8)
### 1.액티비티(Activity)
    사용자와 상호작용을 담당하는 인터페이스
    앱은 하나이상의 액티비티를 가지고 있으며 lifecycle이 존재하여
    관련 메소드 들을 재정의(오버라이딩)할수 있음
### 2.서비스(Service)
    백그라운드에서 동작하는 작업을 처리하기위한 요소로
    별도의 스레드가 아닌 메인(UI)쓰레드 내에서 별도로 생성하여 사용
    -네트워크 연동 가능
    -App이 종료되어도 백그라운드에서 계속 동작
### 3. 방송 수신자 (BroadCast Receiver)
    Aos 로 부터 발생하는 이벤트와정보를 핸들링 하는 컴포넌트
    시스템부팅정보,네트워크끊김,문자수신,배터리 부족등의 정보를
    받아서 처리할 수 있다.
    - 디바이스의 특수한 상황에 대응하기위함
### 4. 콘텐트 제공자 (Content Provider)
    데이터를 관리하고 다른 애플리케이션의 데이터를 제공
    SQLite / Web / File I.O 등을 통해 데이터를 관리
    작은 데이터를 공유하는 intent 와 달리 음악,영상 과같은 용량이 큰 데이터를 공유하기에 적합

### Intent
    컴포넌트간에 정보전달하는 역할 및 통신수단


    