---
layout: single
title: "Conditionl_Q3"
---

[문제 상황]<br>
놀이 공원의 자유이용권 가격을 계산하는 프로그램을 작성하려고 합니다.<br>
요금표는 아래와 같고, 고객의 나이와 입장 시간에따라 금액이 달라집니다.<br>
출력 예를 참고하여 구입요금을 계산하는프로그램을 작성하시오.<br>
단, 시간은 24시간제를 적용하므로 오후 5시는 17시로 표현한다.
![캡처](https://user-images.githubusercontent.com/79987175/120456454-94ae5900-c3d0-11eb-8c12-f894e1202272.PNG)


~~~python
|코드|
Time=float(input('현재 시간을 입력하세요.(24시간제) : '))
Age=float(input('당신의 나이를 입력하세요. : '))
if Time<17:
  if 3<=Age<=12 or Age>=65:
    print('25,000원')
  else:
    print('34,000원')
else:
  print('10,000원')
~~~

|출력 결과|<br>
현재 시간을 입력하세요.(24시간제) : 18<br>
당신의 나이를 입력하세요. : 35<br>
10,000원
