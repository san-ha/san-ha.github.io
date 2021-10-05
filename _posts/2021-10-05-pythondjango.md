---
layout: post
title: Point of Django
subtitle: Python과 Django를 선택한 이유
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [Python, Django]
comments: true
---

## Python 기반

Django는 Python의 특징인 명시성과 간결한 문법, 빠른 생산 속도를 계승한다. 또한 파이썬의 넓은 생태계를 바탕으로 수많은 라이브러리와 높은 확장성을 자랑한다.

다만 Python의 단점인 인터프리터 언어의 느린 속도와 낮은 타입 안정성, 관습의 결핍 또한 상속받는다. 때문에 Django는 내부 속도를 최적화하기 위한 도구들을 제공하며, 여러 도구들을 적용시킬 수 있다.

### Notification

{: .box-note}
**Note:**보다 나은 타입 안정성을 고려한 언어와 프레임워크로는 Kotlin과 Ktor, Swif와 Vapor 등이 있다.



## 정적 페이지 & 동적 페이지

HTML은 정적이고, Python은 동적으로, Django의 템플 태그는 Python을 HTML로 변환하여 정적 페이지와 동적 페이지 모든 유형을 제공한다. 정적 페이지는 미리 저장된 페이지를 그대로 전달하고, 동적 페이지는 서버의 데이터를 사용자의 요청에 따라 가공하여 보여준다.

**정적 페이지 :**
 - 속도가 빠르고 필요한 리소스가 적다
 - 한정된 정보를 출력하며 관리(RUD)가 힘들다.

**동적 페이지 :**
  - 다양한 정보를 조합해 제공하며 관리(RUD)가 쉽다.
  - 속도가 느리며 웹 서버 이외에도 WAS와 DB가 필요하다.


### Notification

  {: .box-note}
  **Note:**다양한 서비스 제공이 필요없는 경우 정적 사이트를 선택한다. 장고 정적 파일 생성기 'Django Distill'을 이용해 동적 사이트를 정적 사이트로 만들 수도 있지만, 다른 최적화된 프레임워크를 사용하는 것이 일반적이다.



## Admin 페이지

Django에서 기본적으로 제공하는 관리자 페이지는 사용자가 별도의 개발 없이 사용할 수 있어, 최소기능제품(MVP)를 빠르게 구현한 후 수정을 거쳐나갈 수 있다.



## 보안

Django는 CSRF 및 SQL 인젝션 등 다양한 공격을 방지하는 기능을 제공한다.



## 프론트엔드 & 백엔드
웹 어플리케이션을 생성할 때 별도의 프레임워크 필요없이, Django 하나로 완성할 수 있다.

다만 Django가 최선은 아니다. 실시간 기능의 낮은 편의성, 동기 비동기 등 벡그라운드 작업 도구 제공 미흡, 동적 페이지 로딩으로 인한 페이지 전환 시 미흡한 사용감, 동적 페이지 로딩 개선 모듈의 낮은 편의성 등 여러 단점들이 존재한다.

### Notification

{: .box-note}
**Note:** Django에서는 실시간 기능을 지원하는 API 'Channels'를 지원하며, 실시간 기능이 뛰어난 프레임워크로 Meteor가 있다.
'Celery'를 사용해 Django가 제공하지 않는 벡그라운드 작업을 처리할 수 있다. 다만 비교적 복잡하고 오버헤드가 커진다.
프레임워크 Gatsby는 기본적으로 페이지 전환이 매끄럽도록 구현하고 있다.
Django에도 동적 페이지 로딩 개선(SSR)을 지원하는 확장 모듈이 존재한다.




## 독립적인 APP으로 인한 다양한 확장

하나의 APP은 별도의 독립적인 환경을 구성하고, 각각의 모델, 템플릿, 뷰를 가진다. 이를 통해 분담 개발이 편리하게 하고, 유용한 확장들을 사용할 수 있도록 한다.

### Notification

{: .box-note}
**Note:**Django Extensions, Django Debug Toolbar, Rosetta, Django REST Framework, 검색, 캐싱, 이미지 변환, CDN 지원 등 수많은 확장 모듈이 존재한다.



## 결론

Django의 여러가지 장점들은 '표준화된 웹 어플리케이션'의 개발 속도를 높혀준다.



## 참조
https://blog.lxf.kr/2018-11-19---why-or-not-django/
https://mungto.tistory.com/302/
http://blog.wishket.com/
https://rakjido.github.io/2020/11/17/Django-Overview/
https://velog.io/@jnine/
