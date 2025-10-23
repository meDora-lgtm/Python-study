# 문제 제목: 영수증 가격 확인

## 문제 정보
- **출처:**
- 백준 문제
- **난이도:**
- medium

## 문제 설명
총 가격이랑 제품 갯수 인풋한다음 다음에 
제품가격과 인풋한 총 금액이 영수증에 찍힌 금액과 같은지 확인하는 문제

## 해결 과정
input으로 total = 0으로 시작하는게 중요

### 접근 방법
마지막에 if 조건문 쓸 때 == 잊지말고 쓰기

## 코드
```python
a = int(input()) #총 영수증 금액
b = int(input()) #물건 갯수

total =0
for i in range(b):
    c, d = map(int, input().split())
    print(c, d)
    total += c*d
    
if total == a:
    print('YES')
else:
    print('NO')
