# 04. 실습 part 1

## A. 알고리즘 문제 해결

## B. 코드 구현

### **I ) 구구단과 계산기**

**예시 코드**

- **구구단**

입력 없이 2 ~ 9단까지 출력

~~~ Python
for n in range(2, 10):
    for m in range(1, 10):
        print(n, 'X', m, '=', n * m)
    print('\n')
~~~

- **계산기**

숫자 두 개 입력받아 계산하기

~~~ Python
# 함수 미사용
print("1. 더하기\n2. 빼기\n3. 곱하기\n4. 나누기\n5. 나머지\n6. 나가기")

while True:
    menu = int(input("원하는 기능 선택: "))
    if (menu < 6):
        Finput = int(input("첫 번째 숫자: "))
        Sinput = int(input("두 번째 숫자: "))
        if(menu == 1):
            print("결과: %d" % (Finput + Sinput))
        elif (menu == 2):
            print("결과: %d" % (Finput - Sinput))
        elif (menu == 3):
            print("결과: %d" % (Finput * Sinput))
        elif (menu == 4):
            print("결과: %d" % (Finput / Sinput))
        elif (menu == 5):
            print("결과: %d" % (Finput % Sinput))
    elif (menu == 6):
        break
    else:
        print("error")
~~~

~~~ Python
# 함수 사용

def add(a, b):
    return a + b
def sub(a, b):
    return a - b
def mul(a, b):
    return a * b
def div(a, b):
    return a / b
def rem(a, b):
    return a % b

print("1. 더하기\n2. 빼기\n3. 곱하기\n4. 나누기\n5. 나머지\n6. 나가기")

while True:
    menu = int(input("원하는 기능 선택: "))
    if (menu < 6):
        Finput = int(input("첫 번째 숫자: "))
        Sinput = int(input("두 번째 숫자: "))
        if(menu == 1):
            res = sum(Finput, Sinput)
            print("결과: %d" % res)
        elif (menu == 2):
            res = sub(Finput, Sinput)
            print("결과: %d" % res)
        elif (menu == 3):
            res = mul(Finput, Sinput)
            print("결과: %d" % res)
        elif (menu == 4):
            res = div(Finput, Sinput)
            print("결과: %d" % res)
        elif (menu == 5):
            res = rem(Finput, Sinput)
            print("결과: %d" % res)
    elif (menu == 6):
        break
    else:
        print("error")
~~~