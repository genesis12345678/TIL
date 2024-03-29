# 자료 구조

### 자료구조란

---
> **Data Structure** : 컴퓨터가 데이터를 효율적으로 다룰 수 있게 도와주는
> 데이터 보관 방법과 데이터에 관한 연산의 총체를 뜻한다.<br>
> 더 정확히 말해, 자료 구조는 데이터 값의 모임, 또 데티어 간의 관계, 그리고
> 데이터에 적용할 수 있는 함수나 명령을 의미힌다. 신중히 선택한 자료구조는 보다 효율적인
> **알고리즘**을 사용할 수 있게 한다.

자료구조는 그림과 같이 ``단순 자료구조``와 ``복합 자료구조``로 나뉜다.<br>
int나 long같은 기본 데이터 형식도 자료구조가 될 수 있다.

![img.png](image/img.png)

복합 자료구조는 다시 ``선형 자료구조``와 ``비선형 자료구조``로 나뉜다.<br>
**선형 자료구조는 데이터 요소를 순차적으로 연결하는 자료구조로 구현하기도 쉽고 
사용하기도 쉽다.**<br>
**비선형 자료구조는 데이터 요소를 비순차적으로 연결한다. 한 데이터 요소에서 여러 데이터
요소로 연결되기도 하고, 여러 데이터 요소가 하나의 데이터 요소로 연결되기도 한다.**

자료구조와 관련해서 알아두면 좋은 개념이 있는데 바로 ADT(Abstract Data Types), 추상 데이터 형식이다.
이것은 자료구조의 동작 방법을 표현하는 데이터 형식이다. 즉 ADT는 자료구조가 갖춰야 할
일련의 연산이라고 할 수 있다.

![img_1.png](image/img_1.png)

### 알고리즘

---

> 어떤 문제를 해결하기 위해 사용되는 풀이과정. 즉 **문제해결방법**을 말한다.
>
> 여러가지 문제해결방법 중 **가장 효율이 좋은 방법**을 **어떤 문제에 대한 알고리즘**이라고 한다.

<br>
<br>

### 시간 복잡도 점근 표기법

---

> **시간복잡도** : 입력값과 문제를 해결하는 데 걸리는 시간을 **함수 관계**로 나타낸 것.
> 즉 실행시간을 기준으로, 알고리즘이 **얼마나 효율적인 지**를 판단할 수 있는 척도이다.

- 최상의 경우 : 오메가 표기법(Big-Ω Notation)
- 평균의 경우 : 세타 표기법(Big-θ Notation)
- **최악의 경우 : 빅오 표기법(Big-O Notation)**

알고리즘을 구할 때는 항상 최악의 경우를 생각해서 구해야 하기 때문에 보통 빅오 표기법을 많이 사용한다.

<br>
<br>

- 선형

    - [배열](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/Array/Array.md)
    - [연결 리스트(링크드 리스트)](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/linkedList/LinkedList.md)
    - [스택](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/stack/Stack.md)
    - [큐](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/queue/Queue.md)
    - [데크](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/dequeue/Deque.md)
    - [해시 테이블](https://github.com/genesis12345678/TIL/blob/main/dataStructure/linear/hash/hash.md)

- 비선형

    - [그래프](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/graph/graph.md)
    - [힙](https://github.com/genesis12345678/TIL/blob/main/dataStructure/non_linear/heap/heap.md)
 