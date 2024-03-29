# 배열과 리스트 예제 - 1

### [문제(백준(1546번) - 평균)](https://www.acmicpc.net/problem/1546)


### 문제 분석
- 최고 점수를 기준으로 전체 점수를 다시 계산해야 하므로 모든 점수를 입력받은 후에 최고점을 별도로 저장해야 한다.
- 문제에서 제시한 한 과목의 점수를 계산하는 식은 총합과 관련된 식으로 변환할 수 있다.
  - 점수가 A, B, C인 경우: `A / M * 100 + B / M * 100 + C / M * 100) / 3` = `(A + B + C) * 100 / M / 3`

### 손으로 풀어보기

1. 점수를 리스트에 저장한다.
2. 리스트를 탐색하며 최고 점수와 점수의 총합을 구한다.
3. `총합 * 100 / 최고 점수 / 과목의 수`를 계산해 정답을 출력한다.

### 슈도코드
```text
n에 과목의 수 입력
list에 점수 정보 저장
max에 점수 정보 중 최댓값 저장
sum에 list 모든 데이터 값 더하기
sum * 100 / max / n 출력
```

### 코드 구현
```python
n = int(input())
myList = list(map(int, input().split()))
myMax = max(myList)
mySum = sum(myList)

print(mySum * 100 / myMax / n)
```