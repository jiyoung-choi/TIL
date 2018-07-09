# Today I Learned
[**파이썬 자습서**](https://docs.python.org/ko/3/tutorial/index.html)를 정독하고 요약하겠습니다.


## [**3장. 파이썬의 간략한 소개**](https://docs.python.org/ko/3/tutorial/introduction.html)

### 마지막에 인쇄된표현식은 변수 ```_```에 대입된다. 즉,
```
tax = 12.5 / 100
price = 100.50
price * tax 
12.5625
price + _
113.0625
round(_, 2)
113.06
```
값을 직접 대입하지 말라고 한다. 
-- 그렇게 한다면 같은 이름의 지역 변수를 새로 만드는 것이 되며, 
내장 변수의 마술 같은 동작(?)을 차단하는 결과를 낳는다고.
[**도무지 무슨말인지 지금은 모르겠지만 미래의 똑똑한 나를 위해 관련 내용(으로 추정되는) 첨부.**](https://nyanye.com/python/2017/01/12/Python-built-in-variables/)

### print()를 사용할때 \n 은 새로운 라인을 만든다.
```
>>> print('First line.\nSecond line.')
First line.
Second line.
```

### 슬라이스가 동작하는 방법

```
 +---+---+---+---+---+---+
 | P | y | t | h | o | n |
 +---+---+---+---+---+---+
 0   1   2   3   4   5   6
-6  -5  -4  -3  -2  -1
```

## [**4장. 기타제어 흐름 도구**](https://docs.python.org/ko/3/tutorial/controlflow.html)

### 4.1. if 문

```
if 조건문:
  수행할 문장 1
  수행할 문장 2
else:
  수행할 문장 A
  수행할 문장 B
```
[예문](https://wikidocs.net/20)
```
money = 1
if money:
    print("택시 타기")
else:
    print("뚜벅이")
```
* : 를 빼먹는 경우가 많으니 주의할 것.

[예문 2]
```
x = int(inpur("please enter an interger: "))
if x < 0:
    x = 0
    print(Negative changed to zero')
elif x == 1:
    print('Single')
else:
    print('More')
```

? 왜 ==를 두번 쓰는 거지 ?

### 4.4. 루프의 break와 continue문 그리고 else 절

break문은 가장 가까이서 둘러싸는 for나 while 루프로부터 빠져나가게 만든다.
```
for n in range(2,10):
    for x in range(2,n):
        if n % x == 0:
            print(n, 'equals', x, '*', n//x)
            break
    else:
        print(n, 'is a prime number')
```

### 4.5. pass 문
문법적으로 문장이 필요하지만 프로그램이 특별히 할 일이 없을때 사용한다.

```
while true:
    pass
```
혹은
```
def initlog(*args):
    pass
```

## 추가로 배운것
- len()
객체의 길이(항목 수)를 돌려준다. 


## [**용어 정리**]
- 리터럴(literal)
- [int](https://docs.python.org/ko/3/library/functions.html#int)
- 이스케이프 : ' 나 "를 그대로 전달하면 에러가 나지만 이스케이프 \' 또는 \"를 한후 전달하면 에러 없이 이스케이프 해제된 문자열을 전달받을 수 있다.
- 슬라이스 : 가져오고 싶은 문자열의 범위를 지정해서 출력하는 것.
- 스트링(string) : 문자열
- 이터레이션 (Iteration): 반복 
- [독스트링(docstring)](https://www.youtube.com/watch?v=HO_hquCSivY) : 함수가 어ㅏ떤일을 수행하는지 설명
```
def 함수이름(인자1,...):
    """함수에 대한 설명"""
    실행할 명령1
    실행할 명령2
    ...
    return 결과
```
- 리스트

