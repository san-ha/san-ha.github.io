---
layout: post
title: Django 만의 차별성
subtitle: Python과 Django를 선택한 이유
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [Python, Django]
comments: true
---

## Python 기반

Django는 Python의 특징인 명시성과 간결한 문법, 빠른 생산 속도를 계승한다. 또한 파이썬의 넓은 생태계를 바탕으로 수많은 라이브러리와 높은 확장성을 자랑한다.

다만 Python의 단점인 인터프리터 언어의 느린 속도와 낮은 타입 안정성 또한 상속받는다. 때문에 Django는 내부 속도를 최적화하기 위한 도구들을 제공하며, 여러 도구들을 적용시킬 수 있다.

보다 나은 타입 안정성을 고려한 언어와 프레임워크로는 Kotlin과 Ktor, Swif와 Vapor 등이 있다.


## 정적 페이지 & 동적 페이지

HTML은 정적이고, Python은 동적으로, Django의 템플 태그는 Python을 HTML로 변환하여 정적 페이지와 동적 페이지 모든 유형을 제공한다. 정적 페이지는 미리 저장된 페이지를 그대로 전달하고, 동적 페이지는 서버의 데이터를 사용자의 요청에 따라 가공하여 보여준다.

**정적 페이지 :**
 - 속도가 빠르고 필요한 리소스가 적다
 - 한정된 정보를 출력하며 관리(RUD)가 힘들다.

**동적 페이지 :**
  - 다양한 정보를 조합해 제공하며 관리(RUD)가 쉽다.
  - 속도가 느리며 웹 서버 이외에도 WAS와 DB가 필요하다.


다양한 서비스 제공이 필요없는 경우 정적 사이트를 선택한다. 장고 정적 파일 생성기 'Django Distill'을 이용해 동적 사이트를 정적 사이트로 만들 수도 있지만, 다른 최적화된 프레임워크를 사용하는 것이 일반적이다.



## Admin


## 참조
https://blog.lxf.kr/2018-11-19---why-or-not-django/
https://mungto.tistory.com/302/
http://blog.wishket.com/
https://rakjido.github.io/2020/11/17/Django-Overview/
https://velog.io/@jnine/
