# 02. 파이썬 설치하기  

## A. 파이썬 설치하기

### **I ) 파이썬 설치하기**

**설치 방법**

파이썬은 파이썬 홈페이지에서 무료로 다운 받을 수 있다.

파이썬 홈페이지 : http://www.python.org

**윈도우 설치 방법**

윈도우는 이곳에서 최신판을 설치한다.  
윈도우가 아니면 위의 파이썬 홈 페이지에서 다른 OS용으로 설치하면 된다.

다운로드 : http://www.python.org/downloads

다운로드 후에 설치 파일을 열어 파이썬을 설치하면 된다.  
이때, 환경 변수 설정이 있는데 이런 것을 잘 모르는 사람은 환경 변수 설정을 해놓으면 좋다.

### **II ) IDE 선택하기**  

01. IDLE

02. Visual Studio Code

03. PyCharm

### **III ) 파이썬 버전 확인하기**

**윈도우에서 하는 방법**

환경 변수를 설정한 사람이라면 cmd(명령 프롬프트)에 Python을 치면 현재 버전과 대화형 쉘 형식으로 파이썬 해석기가 실행될 것이다.

~~~ md
C:\user\legen> Python
>>> print("Hello")
Hello
~~~

환경 변수를 설정하지 않은 사람은 cmd(명령 프롬프트)에 설치한 파이썬의 위치에 경로를 입력한 뒤 하면 된다.

~~~ md
C:\user\legen> cd (파이썬 다운로드 위치)
(파이썬 다운로드 위치)> Python
>>> print("Hello")
Hello
~~~

### **IV ) 출력해보기**

- Hello World

~~~ python
print("Hello world")
~~~