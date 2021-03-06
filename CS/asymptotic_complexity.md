# 시간 복잡도

알고리즘 문제를 풀거나 기술 면접에서 자주 듣게 되는 단어인 **시간 복잡도**.

대충 의미는 파악하고 있지만 정확히는 모르고 있어 이번 기회에 한번 정리해보고자 한다.





## 시간 복잡도란?

프로그래밍에서 시간 복잡도는 **알고리즘이 어떤 문제를 해결하는데 걸리는 시간**을 의미한다.

일반적으로 효율적인 코드는 **시간 복잡도가 작은 코드**를 의미한다.



보통 처음 프로그래밍을 접하는 사람들은 **'효율적인'** 코드의 필요성을 잘 느끼지 못한다. 

왜냐하면 프로그래밍을 배우는 과정에서는 코드를 어떻게 짜든 실행하는 데에 큰 차이가 없기 때문이다.

그저 결과만 정상적으로 나오면 잘 짜여진 코드라고 생각하기 마련이다.



하지만 연산의 횟수가 많아지면, 이를 체감할 수 있게된다.

| 빅-오 표기법 |    1 |    4 |                  16 |                  64 |
| :----------: | ---: | ---: | ------------------: | ------------------: |
|     O(1)     |    1 |    1 |                   1 |                   1 |
|   O(log n)   |    0 |    2 |                   4 |                   6 |
|     O(n)     |    1 |    4 |                  16 |                  64 |
|  O(n log n)  |    0 |    8 |                  64 |                 384 |
|   O($n^2$)   |    1 |   16 |                 256 |                4096 |
|   O($n^3$)   |    1 |   64 |                4096 |              262144 |
|   O($2^n$)   |    2 |   16 |               65536 | 약$1.844 * 10 ^ 19$ |
|    O(n!)     |    1 |   24 | 약$2.092 * 10 ^ 13$ |  약$1.27 * 10 ^ 89$ |

표에서 아래로 갈수록, n이 커질수록 알고리즘의 수행 시간이 기하급수적으로 증가한다.



집에서 혼자 사용하는 경우에는 오래 걸리더라도 큰 문제가 없겠지만,

남과 협업을 하거나 실제로 서비스를 운영하는 입장에서는 매우 큰 부담이 될 수 밖에 없다.





## 표기법

빅-오(Big-Oh) / 빅-세타(Big-Theta) / 빅-오메가(Big-Omega)





### 빅-오(Big-Oh) 표기법

알고리즘의 시간 소모의 상한
컴퓨터 프로그래밍에서 널리 사용되는 표기법.
알고리즘의 평균적인 시간은 의미가 없는 경우가 많다.
평균적으로 걸리는 시간 보다는, 상한을 알려주는 것이 더 믿음직스럽다.





### 빅-세타(Big-Theta) 표기법

알고리즘의 평균적인 시간





### 빅-오메가(Big-Omega) 표기법

알고리즘의 최선의 시간





## 공간복잡도

그렇다면 시간 복잡도가 작은 알고리즘이 무조건 좋은가

공간복잡도는 알고리즘을 수행해서 메모리가 얼마나 필요한가를 표기하는 것



