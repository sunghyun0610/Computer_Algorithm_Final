💻Computer Algorithm final-term assingment💻
<br> by 201901671 문성현
===========================================

# Topic : ~에 따른 ~의 변화를 최적해 알고리즘(유전 알고리즘,SA(simulated Annealing))을 이용해 알아보고 회기식과의 오차를 알아본다.

## List
- **1.최적해(유전)알고리즘 원리 및 설명**
    - *1-1. P&Np(NP-hard)문제 소개*
    - *1-2. 용어 정리(사전지식) 및 유전알고리즘 원리 설명*
    - *1-3. 유전 알고리즘을 이용해 주제(topic)의 최적해 구하기*
- 2.**유전(Genetic) 알고리즘으로 주제 구현(C++) 및 동작방식 설명**
- **3.코드 결과 및 성능 분석**
- **4.개선점과 하면서 새로 배우고 느낀 점**
<br><br>
## 1-1 P&NP(NP-hard)문제 소개
### P 문제는 결정 문제들 중에서 쉽게 풀리는 것을 모아 놓은 집합이다. 어떤 결정 문제가 주어졌을 때, 다항식(Polynomial) 시간 이내에 그 문제의 답을 YES와 NO 중의 하나로 계산해낼 수 있는 알고리즘이 존재하는 문제이다.
### 수업시간에 다루었던 NP(Non-deterministic Polynomial) 문제는 형식적으로는, 문제를 푸는 각 단계에서 여러가지의 가능성을 동시에 고려할 수 있는 비결정적 알고리즘(non-deterministic algorithm)으로 다항시간내에 문제를 해결할 수 있는 문제라고 정의한다.

