# Today I Leanred

[**ewith 모두를 위한 프로그래밍 : 파이썬 (py4e)**](https://www.edwith.org/pythonforeverybody)

## CHAPTER 2. 변수, 표현식 및 코드
### 연산자, 데이터 타입 및 타입 변환

1. Type Matters

```
>>> ddd = 1 + 4
>>> print(ddd)
5
>>> type(1)
<class'int'>

>>> eee = 'hello ' + 'there'
>>>print(eee)
hello there
>>> type(hello)
<class'str'>
>>> type(eee)
<class'str'>
```
* int(integer) = 정수
* str(string) = 문자열


2. User Input

```
>>> nam = input('Who are your? ")
>>> print('Welcome', nam)

Who are you? ~Chuck~
Welcome Chuck
```
* input()는 사용자가 입력값을 넣을때까지 기다리는 함수


3. [실습] 

- 프롬프트에서 사용자 입력(input) 받기
```
nzt = input('Enter your name: ')
print("Hello",nzt)
```

* command + k : 터미널 창 클리어

- 프롬프트에서 입력받아 계산하기

```
xh = input("Enter Hours: ")
xr = input("Enter Rate: ")
xp = float(xh) * float(xr)
print("Pay:",xp)
```

line 3에서 float()를 하지 않으면 xh, xr값이 숫자로 넣었다고 하더라도 기본으로 문자열(String)로 입력되기 때문에
숫자로 변경해줘야함.
print("Pay:",xp)기본 
print("Pay:",xp)
