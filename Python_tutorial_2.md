# Today I Learned
[**파이썬 자습서**](https://docs.python.org/ko/3/tutorial/index.html)를 정독하고 요약하겠습니다.
3장부터 4장 4.5. pass문은 [여기](https://github.com/jiyoung-choi/TIL/blob/master/Python_tutorial_1.md)로.

## [**4장. 기타 제어 흐름 도구**](https://docs.python.org/ko/3/tutorial/controlflow.html)

### 4.6. 함수 정의하기

출처 : [점프 투 파이썬 위키독스](https://wikidocs.net/24)
```
def 함수명(매개변수):
    <수행할 문장1>
    <수행할 문장2>
    ...
```

즉,
```
def sum(a, b):
    return a+b
    
print(sum(3,4))
```

튜토리얼에서는 피보나치 수열을 임의 한도까지 출력하는 함수를 만들었다.
```
def fib(n)
    a, b = 0, 1
    while a < n
        print(a, end='')
        a, b = b, a+b
    print()
    
fib(2000)
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610 987 1597
```

```
def ask_ok(prompt, retries=4, reminder='please try again!'):
    while True:
    ok = input(prompt) 
```



## [용어 정리]
- 스코프(scope): 유효 범위, 변수의 수명(변수가 유효한 범위)를 의미한다. [*참고](http://justmakeyourself.tistory.com/entry/python-scope)
- 
