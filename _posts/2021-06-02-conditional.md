---
layout: single
title: "Conditionl_Q1"
---

[문제 상황]<br>
가위, 바위, 보 게임을 만들어 봅시다.<br>
가위바위보 게임은 다음과 같이 진행됩니다.<br>
ex1)<br>
나 입력(가위:s, 바위:r, 보:p): s<br>
너 입력(가위:s, 바위:r, 보:p): s<br>
비겼다.<br>
ex2)<br>
나 입력(가위:s, 바위:r, 보:p): r<br>
너 입력(가위:s, 바위:r, 보:p): s<br>
이겼다.
ex3)<br>
나 입력(가위:s, 바위:r, 보:p): p<br>
너 입력(가위:s, 바위:r, 보:p): s<br>
졌다.

~~~python
|코드|
#가위:s, 바위:r, 보:p
a=input('나 : ')
b=input('상대방 : ')
if a=='s' and b=='p' or a=='r' and b=='s' or a=='p' and b=='s':
  print('이겼다.')
elif a=='s' and b=='r' or a=='r' and b=='p' or a=='p' and b=='r':
  print("졌다.")
elif a==b:
  print('비겼다.')
~~~

|출력 결과|<br>
나 : s<br>
상대방 : p<br>
이겼다.
