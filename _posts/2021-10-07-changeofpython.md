---
layout: post
title: Change of Python
subtitle: Python2와 Python3의 차이점
cover-img: /assets/img/coding.jpg
thumbnail-img: /assets/img/python.png
share-img: /assets/img/coding.jpg
tags: [Python]
comments: true
---

## 업데이트

Python2는 2020.01.01 이후로 더 이상 업데이트 없이 최종 2.7 버전으로 마감하였다. Python3는 지속적으로 새로운 버전이 출시되고 있다.  




## 문자열 데이터 타입

Python2는 문자열 데이터 타입이 ASKII(Bytes)인 반면, Python3는 Unicode를 사용하여 다양한 나라의 언어를 표현할 수 있게 되었다.

{: .box-note}
Python2는 Bytes(8bit)로 알파벳을 나타내는 것에 중점을 두어 다른 언어 표현에 제약이 있었으나, 별도의 설정을 통해 Unicode 방식을 지원하였다.

{: .box-warning}
문자열 데이터 타입이 달라짐에 따라 Python2의 프로그램이 Python3에서 에러가 발할 수 있다.




## print문
Python2 에서는 괄호가 없어도 출력이 가능하였으나, python3에서는 print문이 함수로 동작하므로 괄호가 반드시 필요하다.
~~~
print('hello')
print'hello
#hello
~~~
~~~
print('hello')
#hello
~~~




## 정수형 계산 결과
Python2에서는 정수형의 계산결과는 정수형이였으나, Python3에서는 실수형이 출력된다.
~~~
sum = 5/2
print( sum )
# 2
~~~
~~~
sum = 5/2
print( sum )
# 2.5
~~~




## 정수형 int로 통일
Python2에서는 긴 정수형의 경우 long 타입을 사용하였으나, Python3에서는 int로 통일하였다.  




## 이외에도
Garbage Collection 및 메모리 할당기능이 개선되는 등 여러 사항이 변경되었다.




## 참조
https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=nackji80&logNo=221597433538  
https://zetawiki.com/wiki/Python_%EB%B2%84%EC%A0%84_2%EC%99%80_3_%EC%B0%A8%EC%9D%B4  
https://ojava.tistory.com/169  
https://jins-dev.tistory.com/entry/Python-2-%EB%B2%84%EC%A0%84%EA%B3%BC-3-%EB%B2%84%EC%A0%84%EC%9D%98-%EC%B0%A8%EC%9D%B4  
