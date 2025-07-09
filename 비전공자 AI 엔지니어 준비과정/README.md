# AI 공부 로그 (study-log)

안녕하세요!  
비전공자로서 AI 엔지니어가 되기 위해 공부하고 기록하는 저장소입니다.

## 학습 로드맵

1. Python 기초 문법 및 활용  
2. 데이터 분석 (Pandas, Numpy, 시각화)  
3. 머신러닝 기본 알고리즘 (선형 회귀, 분류, 트리 등)  
4. 딥러닝 기초 (신경망, CNN, RNN)

## 현재 진행 상황

- Python 기초 강의 수강중  

---

## 공부 방식

- 강의 수강 → 실습 코드 작성 → 주요 내용 정리 → 커밋 기록  
- 모르는 부분은 이슈로 기록해 다시 복습  

---

## 저장소 구성

- 01_python_basics: 파이썬 기초 문법 및 간단한 예제 코드  
- 02_data_analysis: 데이터 처리 및 시각화 관련 실습  
- 03_machine_learning: 머신러닝 알고리즘 코드  
- 04_deep_learning: 딥러닝 기본 모델 및 실습

---

#수정필요

폴더구조
study-log/
├─ README.md
├─ 01_python_basics/
│   ├─ hello_world.py
│   ├─ variables_and_types.py
│   └─ README.md
├─ 02_data_analysis/
│   ├─ pandas_tutorial.ipynb
│   ├─ numpy_examples.py
│   └─ README.md
├─ 03_machine_learning/
│   ├─ linear_regression.py
│   ├─ decision_tree.py
│   └─ README.md
└─ 04_deep_learning/
    ├─ neural_network_basic.py
    ├─ cnn_example.ipynb
    └─ README.md


## 연락처

궁금한 점이나 피드백은 이메일(youremail@example.com)로 연락 주세요.

#25.07.06 일
print("hello, world!")
print("hello")
# print("ctrl + / 입력 시 주석이 되어 컴퓨터는 읽지 못하게 할 수 있습니다. or #을 입력 후 작성하면 읽지 못하게 할 수 있습니다.")
# print("다시 ctrl + / 입력 시 주석이 되어있던걸 풀 수 있습니다.")
# 실행버튼 단축키는 f5는 디버깅을 사용하면서 실행하는거고 ctrl + f5 누르면 실행이 됩니다.
'''
아래 코드는 hello world를 출력하는 코드입니다.
테스트
'''
# 은 진짜 주석, """은 실제 주석이 아니라 문자열 여러 줄 설명 할때 사용


#25.07.08 화

### 자료형
# 1+1=2 이지만 자료형에 따라 2가 아닌 경우가 있다 '1'+'1'='11' '1' 자체가 문자인 경우 문자열을 붙인다는 개념으로 '11'이 된다.
# 자료형에는 (숫자, 문자열, 불), (변수, 리스트, 튜플, 딕셔너리, 집합)이 있습니다.

### 변수
# 변수란 상자개념 상자안에 값을 담는다라고 이해하면 편합니다.
# a=3은 같다는 개념이 아니라 a안에 3을 담는다는 개념입니다.

### 숫자형
# 정수형(1, 2, -2) int, 실수(1.24, -34.56) float
# 컴퓨터식 지수 표현 방식(4.24e10, 4.24e-10), 8진수(0o37), 16진수(0x7a)
# 주로 정수형, 실수를 많이 사용함

# 정수(출력 값 int)
a=123
print(type(a))

# 실수(출력 값 float)
a=1.2
print(type(a))

a=4.24e10 #e10은 e에 10승 이런 개념
print(type(a))

# 실수형이지만 실행 시킨 후 TERMINAL에 cls 입력 후 정리하는 작업 실습
a=4.24e10 
print(a)

### 사칙 연산(+ , - , / , *)
a=3
b=4
print(a-b)

# x의 y제곱을 나타내는 ** 연산자
a=3
b=4
print(a**b)

# 나눗셈 후 나머지를 리턴하는 % 연산자(나머지를 구하는 법)
print(7%3)

# 나눗셈 후 몫을 리턴하는 // 연산자(몫을 구하는 법)
print(7//3)

### 문자열

## 문자열 자료형 만드는 4가지 방법

# 1. 큰따옴표로 양쪽 둘러싸기
# 2. 작은따옴표로 양쪽 둘러싸기
# 3. 큰따옴표 3개를 연속으로 써서 양쪽 둘러싸기
# 4. 작은따옴표 3개를 연속으로 써서 양쪽 둘러싸기

a = "Life is too shrt, you need Pythoon"
b = "a"
c = "123"
print(type(a))
# 입력시 <class 'str'> 입력 [str = string = 문자열 자료형의 약자]
# 1은 숫자이지만 "1"은 문자열이 되어 붙음

a = 'Life is too shrt, you need Pythoon'
print(type(a))

## 따옴표안에 다른 따옴표 넣는 방법 
a = "Life ' is too shrt, you need Pythoon"
b = 'Life " is too shrt, you need Pythoon'
print(type(a))

## 같은 따옴표를 넣는 방법
a = "Life\" is too shrt, you need Pythoon"
print(a)
# \ 가 특수기호 역할을 하여 따옴표가 중복되도 끝나지 않음

## 여러 줄인 문자열을 변수에 대입하는 방법(줄바꿈)
# 1. 줄을 바꾸기 위한 이스케이프 코드 \n 삽입하기
a = "Life is too shrt \nyou need Pythoon"
print(a)

# 2. 문자 시작과 끝에 """ or ''' 삽입하여 줄 바꾸기 실행
a = """Life is too shrt 
you need Pythoon"""
print(a)
# 실행하면 """ Life is too shrt
#             you need Pythoon"""로 출력

## 이스케이프 코드 : 프로그래밍할 때 사용할 수 있도록 미리
# 정의해 둔 '문자 조합'을 말함

## 이스케이프 코드 설명
# \n : 문자열 안에서 줄을 바꿀 때 사용

# \t : 문자열 사이에 탭 간격을 줄 때 사용(자주 사용x)
a = "Life is too shrt \tyou need Pythoon"
print(a)
# 출력값 Life is too shrt      you need Pythoon

# \\ : \를 그대로 표현할 때 사용
a = "Life is too shrt \\you need Pythoon"
print(a)
# 출력값 Life is too shrt \you need Pythoon

# \' : 작음따옴표를 그대로 표현할 때 사용
# \" : 큰따옴표를 그대로 표현할 때 사용

# 아래는 프로그램에서 잘 사용하지 않음
# \r : 캐리지 리턴(줄 바꿈 문자, 커서를 현재 줄의 가장 앞으로 이동)
# \f : 폼 피드(줄 바꿈 문자, 커서를 현재 줄의 다음 줄로 이동)
# \a : 벨 소리(출력할 때 pc 스피커에서 '삑' 소리가 난다)
# \b : 백 스페이스
# \000 : 널 문자

## 문자열 연산

## 문자열 더해서 연결하기
head = "python"
tail = " is fun!"
print(head + tail)
# 출력값 python is fun!

## 문자열 곱하기(반복해서 붙인다)
a= "python"
print(a*3)
# 출력값 pythonpythonpython

## 문자열 곱하기 응용하기
# multustring.py
print("="*50)
print("My Program")
print("="*50)
# 반복된 문자를 빠르게 입력 가능하게 됨 

## 문자열 길이 구하기(띄어쓰기 수도 포함)
a = "Life is too short"
print(len(a))

## 문자열 인덱싱과 슬라이싱
a = "Life is too short, you need Python"
print(a[3])
# 출력값 e
# 인덱싱 : 문자열를 1개씩 뽑아오는 기능
# 문자열 순서대로 카운팅 시작은 0 단위로 시작, 공백도 카운터 됨

## 문자열 활용
a = "Life is too short, you need Python"
print(a[0])
print(a[12])
print(a[-1]) # -1은 문자열에 역순으로 시작
# 출력값 "L", "s", "n" 

## 문자열 슬라이싱 : 범위를 정해서 가져오는 기능
a = "Life is too short, you need Python"
b = a[0:4]
print(b)
# 출력값 Life
# a[a이상 : b미만 : c간격] " : "가 1개 일시 이상 미만만 사용

# a[시작_번호:끝_번호]에서 끝 번호 부분을 생략하는 방법
a = "Life is too short, you need Python"
b = a[19:] # 끝 번호를 생략할 시 문자열 끝까지 지정하여 가져옴
print(b)
# 출력값 you need Python

# 간격 적용 방법
a = "Life is too short, you need Python"
b = a[::2] # 문자열 2칸씩 띄고 가져옴
print(b)

a = "Life is too short, you need Python"
b = a[::-1] # 거꾸로 가져옴
print(b)

a = "Life is too short, you need Python"
b = a[::-2] # 거꾸로 2칸씩 띄고 가져옴
print(b)

# 슬라이싱에서 인덱싱 적용하는 방법

a = "20230331Rainy"
date = a[:8] 
weather = a[8:]
print(date)
print(weather)
# 출력값 "20230331", "Rainy"

## 문자열 포매팅
# 문자열 포매팅 : 특정 문자열을 바꾸고 싶을때 사용하는 기술

# 1. 숫자 바로 대입
a = "I eat %d apples." % 3 
print(a)
# 출력값 I eat 3 apples
# %d란 decimal [데시마일(십진의)] 문자를 쓰고 %뒤에 숫자를 가져옴

# 2. 문자열 바로 대입
a = "I eat %s apples." % "five" 
print(a)

# 3. 숫자 값을 나타내는 변수를 대입
number = 3
a = "I eat %d apples." % number 
print(a)

# 4. 2개 이상의 값 넣기
number = 3
day = "theree"
a = "I eat %d apples. so I was sick for %s day" % (number,day) 
print(a)
