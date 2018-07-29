# Today I Learned

최성철 교수의 ''머신러닝을 위한 파이썬'' 수업 중 Data handling = Pandas #1를 수강하고 작성한 노트입니다.



## Pandas란?

- 구조화된 데이터의 처리를 지원하는 Python 라이브러리
- Array 계산 라이브러리인 Numpy와 통합하여 스프레드시트 처리 기능을 제공

```
import pandas as pd		 # 라이브러리를 호출한다. 참고. pd : Pandas의 약어
df_data.head()			# 데이터의 처음 다섯줄을 출력한다.
df_data.values			# Numpy 형태의 값을 출력.

```

- Series(Numpy에서 하나의 벡터, DataFrame 중 하나의 Column/Row에 해당하는 데이터)와 DataFrame(Data Table 전체)이라는 Object로 구성되어 있다.

## Pandas 실습

- 주피터에서 Shift + Tab
- Index의 이름을 지정, 이름을 통해 값을 불러올 수 있다.

```
raw_data = {'first_name':['Jason', 'Molly', 'Tina', 'Jake', 'Amy'],'last_name':['Miller', 'Jacobson', 'Ali', 'Milner', 'cooze'], 'age':[42, 52, 36, 24, 73], 'city': ['San Francisco', 'Baltimore', 'Miami', 'Douglas', 'Boston']}

df = pd.DataFrame(raw_data, columns = ['first_name', 'last_name', 'age', 'city'])

df
```

|      | first_name | last_name | age  | city          |
| ---- | ---------- | --------- | ---- | ------------- |
| 0    | Jason      | Miller    | 42   | San Francisco |
| 1    | Molly      | Jacobson  | 52   | Baltimore     |
| 2    | Tina       | Ali       | 36   | Miami         |
| 3    | Jake       | Milner    | 24   | Douglas       |
| 4    | Amy        | Cooze     | 73   | Boston        |



```
df.loc()			# loc = index location 값 가져오기 (라벨 값)
df.iloc()			# iloc - index position 값 가져오기 (순서 정수)
```

