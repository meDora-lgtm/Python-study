# Python-study
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
