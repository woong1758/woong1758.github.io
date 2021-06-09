---
layout: single
title: "Infinite-Iteration_Q9"
---

[문제 상황]<br>
요트 경주는 물 위에 부표를 띄워 표시해 둔 코스를 정해진 시간 내에 가장 빨리 완주하는 게임입니다.<br>
육상에서 하는 스포츠와는 다르게 바람, 조류, 파도 등 여러 영향을 많이 받기 때문에 레이스를 여러 번 하여 종합점수로 순위를 정합니다.<br>
5팀이 출전하여 3번의 기록이 다음과 표와 같을 때, 각 팀 기록의 평균을 구하여 출력하는 프로그램을 작성해 보시오.

~~~python
|코드|
Yacht=[['A', 55, 48, 60],['B', 77, 60, 55],['C',49, 65, 60],['D', 70, 58, 63],['E', 54, 50, 58]]
alist=[]

for i in range(len(Yacht)):
  sum=0
  for j in range(1, len(Yacht[i])):
    sum+=Yacht[i][j]
  alist.append(int(sum/(len(Yacht[0])-1)))

for i in range(5):
  print(Yacht[i][0], ':', alist[i])
~~~

|출력 결과|<br>
A : 54<br>
B : 64<br>
C : 58<br>
D : 63<br>
E : 54
