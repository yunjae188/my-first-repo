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

# 자료형
# 1+1=2 이지만 자료형에 따라 2가 아닌 경우가 있다 '1'+'1'='11' '1' 자체가 문자인 경우 문자열을 붙인다는 개념으로 '11'이 된다.
# 자료형에는 (숫자, 문자열, 불), (변수, 리스트, 튜플, 딕셔너리, 집합)이 있습니다.

# 변수
# 변수란 상자개념 상자안에 값을 담는다라고 이해하면 편합니다.
# a=3은 같다는 개념이 아니라 a안에 3을 담는다는 개념입니다.

# 숫자형
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
