# Today I Learned with Djangogirls!

## 정규표현식 (Regex, Regular expressions)

```
^ : 문자열이 시작할 때
$ : 문자열이 끝날 때
\d : 숫자
() : 패턴의 부분을 저장할 때
```

http://www.mysite.com/post/12345/에서 정규표현식으로 url 패턴을 만들어 숫자값과 매칭되게 하려면?
```
^post/(\d+)/$
```
^post/ : url이(오른쪽부터) ```post/```로 시작합니다.
(\d+) : 숫자(한 개 이상)가 있습니다. 이 숫자로 조회하고 싶은 게시글을 찾을 수 있어요.
/ : ```/```뒤에 문자가 있습니다.
$ : url 마지막이 ```/```로 끝납니다.
