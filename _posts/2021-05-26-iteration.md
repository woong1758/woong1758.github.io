---
layout: single
title: "Iteration_Q1"
---

[문제 상황]<br>
스티븐과 그의 여동생 마리는 마을 파티에서 상영할 영화를 구입하기 위해 유튜버 실시간 방송을 하여 슈퍼챗 후원을 받고 있습니다.<br>
모금 목표 금액은 10만원입니다.<br>
10만 이상의 금액이 넘어가면 바로 방송을 종료할 것입니다.<br>
후원금액을 자동으로 관리하는 프로그램을 작성해 봅시다.

~~~python
|코드|
sum=x=0
while sum<=100000:
  x=int(input('후원 금액 : '))
  sum=x
print('방송 종료')
~~~

|출력 결과|<br>
후원 금액 : 1000<br>
후원 금액 : 1000000<br>
방송 종료
