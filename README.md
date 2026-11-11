# CLT-Python

Core Level Tutorial - Python

Python의 문법과 실행 원리를 공부하는 강의 노트와 실습 자료다. 이름과 객체의 관계, 함수 호출, Scope, 모듈의 동작을 코드로 확인한다.

## 학습 흐름

문법 구성요소에서 시작해 문법의 구조, 실행 모델, 코드 설계로 이어진다.

| 구분 | 주제 |
| --- | --- |
| 문법 구성요소 | Token, Literal, Expression, Statement, 객체와 타입, 일급 객체로서의 함수 |
| 문법 구조 | 조건문과 반복문, Iteration Protocol, Comprehension, 들여쓰기와 블록, 함수와 모듈 구조 |
| 실행 모델 | Namespace와 Scope, Stack Frame과 Call Stack, 메모리 관리, Bytecode와 Interpreter |
| 코드 관례와 설계 | Pythonic Idiom, Decorator, Property, Type Hint, 디자인 패턴, Python의 설계 철학 |

GIL과 동시성, 비동기와 Coroutine, Descriptor, Dataclass, 메타프로그래밍은 확장 학습 주제로 둔다.

## 자료 안내

| 자료 | 내용 |
| --- | --- |
| [Python 기본 강의](Lectures/L01_Basic_of_Python/README.md) | 문법, 객체, 함수, Scope, 모듈, 컬렉션, 클래스, 예외 처리 |
| [주차별 실습](Lectures/L02_midterm/) | Python 환경, 제어문과 반복문, Pandas 실습 |
| [Pandas](Lectures/L02_midterm/week05.ipynb) | Series와 DataFrame을 이용한 데이터 처리 |
| [Pillow](Lectures/L05_PIL/) | 이미지 열기와 복사, 그리기, 보정, 필터 |
| [Git](Lectures/L06_Git/) | 저장소 생성, 변경 확인, 커밋, 복원과 되돌리기 |
| [Colab 실습](Lectures/L07_Colab/) | 데이터 분석 과제 |
| [Matplotlib](Lectures/L08_matplotlib/) | 그래프 작성과 시각화 |
| [가상환경](Lectures/venvs/README.md) | Python 환경 구성 관련 노트 |
| [이전 자료](Lectures/Legacy/) | 이전 구성의 강의 노트와 설치 자료 |

기본 개념은 Python 기본 강의의 순서대로 읽고, 도구와 라이브러리 실습은 필요한 자료를 골라 진행한다.

## 실습 환경

프로젝트 설정은 Python 3.13 이상을 기준으로 한다. 의존성은 [pyproject.toml](pyproject.toml)에, 설치 버전은 [uv.lock](uv.lock)에 기록되어 있다.

uv가 설치되어 있다면 저장소 루트에서 다음 명령으로 환경을 구성한다.

```bash
uv sync
```

VS Code에서 `.ipynb` 파일을 열고, 생성된 `.venv`의 Python 인터프리터를 노트북 커널로 선택한다. 다른 노트북 편집기를 사용해도 같은 환경의 커널을 선택하면 된다.

셀은 위에서부터 실행한다. 실행 순서가 섞여 변수나 함수의 상태가 불분명해졌다면 커널을 다시 시작한다. 실습의 `TODO`와 `pass`는 직접 구현하고, 실행 결과를 예상한 뒤 실제 결과와 비교한다.
