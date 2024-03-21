# Python_Tutorial
# 파이선 정리

파이선 변수 선언 및 할당

- 프로그램에서 데이터를 저장하고 참조해야 할 때 사용합니다 변수에 값을 할당함으로써, 해당 값을 나중에 이름을 통해 찾아 사용할 수 있습니다
- 데이터를 저장하고 프로그램의 다른 부분에서 그 데이터를 재사용하기 위함입니다.

파이썬(Python)은 간결하고 읽기 쉬운 문법으로 유명한 프로그래밍 언어입니다. 파이썬을 시작하는 데 필요한 몇 가지 기본적인 문법을 알려드리겠습니다.

1. **변수와 데이터 타입**
    - 변수는 값을 저장하는데 사용됩니다. 변수를 할당할 때 데이터 타입을 명시할 필요가 없습니다.
    
    ```python
    pythonCopy code
    x = 5         # 정수
    y = 3.14      # 부동소수점
    name = "John" # 문자열
    is_true = True # 불리언
    
    ```
    
2. **기본 연산자**
    - 산술 연산자: **`+`**, **``**, **``**, **`/`**, **`//`** (정수 나눗셈), **`%`** (나머지), **`*`** (지수)
    - 비교 연산자: **`==`**, **`!=`**, **`<`**, **`>`**, **`<=`**, **`>=`**
    - 논리 연산자: **`and`**, **`or`**, **`not`**
3. **조건문**
    - 조건에 따라 코드를 실행합니다.
    
    ```python
    pythonCopy code
    if x > 0:
        print("Positive")
    elif x == 0:
        print("Zero")
    else:
        print("Negative")
    
    ```
    
4. **반복문**
    - 코드 블록을 여러 번 실행합니다.
    - **`for`** 루프:
    
    ```python
    pythonCopy code
    for i in range(5):
        print(i)
    
    ```
    
    - **`while`** 루프:
    
    ```python
    pythonCopy code
    i = 0
    while i < 5:
        print(i)
        i += 1
    
    ```
    
5. **함수**
    - 코드를 재사용하기 위해 사용됩니다.
    
    ```python
    pythonCopy code
    def greet(name):
        print("Hello, " + name)
    
    greet("Alice")
    
    ```
    
6. **리스트**
    - 여러 값을 저장하는데 사용됩니다.
    
    ```python
    pythonCopy code
    my_list = [1, 2, 3, 4, 5]
    print(my_list[0])  # 인덱스로 값에 접근
    
    ```
    
7. **딕셔너리**
    - 키-값 쌍을 저장하는데 이루어진 데이터 구조를 사용됩니다.
    
    ```python
    pythonCopy code
    my_dict = {"name": "John", "age": 30}
    print(my_dict["name"])  # "John" 출력
    
    ```
    
8. **문자열 다루기**
    - 문자열을 조작하는데 사용됩니다.
    
    ```python
    pythonCopy code
    my_string = "Hello, world!"
    print(len(my_string))   # 문자열 길이
    print(my_string.upper()) # 대문자 변환
    
    ```
    

이것은 파이썬의 기본적인 문법에 대한 간략한 개요입니다. 파이썬은 매우 다양한 기능을 제공하므로, 더 많은 기능을 배우고 싶다면 파이썬 공식 문서나 다양한 온라인 자료를 참고하는 것이 좋습니다.

1. **리스트 컴프리헨션**
    - 리스트를 만드는 간결한 방법을 제공합니다.
    
    ```python
    pythonCopy code
    squares = [x**2 for x in range(10)]
    
    ```
    
2. **파일 다루기**
    - 파일을 열고 읽거나 쓸 수 있습니다.
    
    ```python
    pythonCopy code
    with open("myfile.txt", "r") as f:
        content = f.read()
    
    ```
    
3. **클래스**
    - 객체 지향 프로그래밍을 지원합니다.
    
    ```python
    pythonCopy code
    class Car:
        def __init__(self, make, model):
            self.make = make
            self.model = model
    
        def info(self):
            print(f"{self.make} {self.model}")
    
    my_car = Car("Toyota", "Corolla")
    my_car.info()
    
    ```
    
4. **모듈과 패키지**
    - 모듈을 사용하여 코드를 구성하고 관리합니다.
    
    ```python
    pythonCopy code
    import math
    print(math.sqrt(25))
    
    ```
    
5. **예외 처리**
    - 예외 상황을 처리할 수 있습니다.
    
    ```python
    pythonCopy code
    try:
        result = 10 / 0
    except ZeroDivisionError:
        print("Cannot divide by zero")
    
    ```
    
6. **내장 함수**
    - 파이썬은 다양한 내장 함수를 제공합니다.
    
    ```python
    pythonCopy code
    print(len([1, 2, 3]))   # 리스트 길이
    print(max(4, 7, 1))     # 최댓값
    
    ```
    
7. **정규 표현식**
    - 문자열 패턴 매칭을 위해 사용됩니다.
    
    ```python
    pythonCopy code
    import re
    pattern = r"\b\w{4}\b"
    print(re.findall(pattern, "This is a test sentence"))
    
    ```
    ![image](https://github.com/Shinjunyeop/Python_Tutorial/assets/159976500/404cf0d7-fd48-47d0-92b9-05877e4f47b4)

8. **라이브러리와 외부 패키지**
    - 파이썬은 다양한 라이브러리와 외부 패키지를 사용하여 기능을 확장할 수 있습니다. 예를 들면, NumPy, Pandas, Matplotlib 등이 있습니다.

위에 제시된 내용은 파이썬의 주요 기능 중 일부에 불과합니다. 더 많은 기능과 세부적인 내용을 알고 싶다면 파이썬 공식 문서 또는 다양한 온라인 자료를 참고하는 것이 좋습니다.
