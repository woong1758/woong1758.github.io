---
layout: single
title: "Infinite-Iteration_Q1"
---

[문제 상황]<br>
DAUM에서는 주기적으로 비밀번호를 변경하여 개인정보를 안전하게 보호하고 있습니다.<br>
ID는 ‘알파벳+숫자’ 의 조합으로, ‘woong1758’과 같이 만들 수 있습니다.<br>
새로 변경하려는 비밀번호에서 연속된 3글자가 ID에 들어있다면 그것은 사용이 허락되지 않습니다.<br>
위에서설명한 것과 같이 비밀번호 변경 가능 여부를 체크한 후에 비밀번호를 변경하는 프로그램을 작성하시오.

~~~python
|코드|
ID='woong1758'
pw=input('Password : ')
for i in range(len(pw)-2):
  if pw[i:i+3] in ID:
    print('사용 불가')
    break
else:
  print('사용 가능')
~~~

|출력 결과|<br>
Password : hwhj1107
사용 가능
