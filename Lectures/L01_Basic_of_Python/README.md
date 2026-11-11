# Basic of Python

Python의 문법과 실행 방식을 다루는 강의 노트다. 이름과 객체의 관계부터 함수 호출, Scope, 모듈 구조까지 예제로 살펴본다.

## 강의 자료

| 순서 | 노트북 | 내용 |
| --- | --- | --- |
| 01 | [Python 언어 구조](L01_python_structure.ipynb) | REPL, Token, AST, Bytecode, Expression과 Statement |
| 02 | [Lexical Structure & Literal](L02_lexical_literal.ipynb) | Keyword, Identifier, Literal, `tokenize`, 명명 규칙 |
| 03 | [Expression & Statement](L03_expression_statement.ipynb) | 연산자 우선순위, 문장의 구조, AST, `eval()`과 `exec()` |
| 04 | [Object Model & Type System](L04_object_type.ipynb) | 이름과 객체, Identity, Mutability, 복사, 타입 체계 |
| 05 | [Control Flow](L05_control_flow.ipynb) | Truthiness, 단락 평가, 조건문, 비교와 멤버십 연산 |
| 06 | [Iteration Protocol](L06_iteration_protocol_notebook.ipynb) | Iterable과 Iterator, 반복문, Generator, Comprehension |
| 07 | [Function & Scope](L07_function_scope_notebook.ipynb) | 함수 호출, 매개변수, 인자 전달, Scope, Closure |
| 08 | [Namespace & LEGB](L08_namespace_scope_legb.ipynb) | 이름 찾기, `global`, `nonlocal`, Shadowing |
| 09 | [Module & Package](L09_module_package_notebook.ipynb) | Import, Package 구조, pip, 가상환경 |
| 10 | [Collection Types](L10_collection_types_lecture.ipynb) | Sequence, Dict, Set, `collections`, 시간·공간 복잡도 |
| 11 | [OOP & Class](L11_OOP_Class_lecture.ipynb) | Class와 Instance, Special Method, 상속, 다형성, Property |
| 12 | [Exception Handling & I/O](L12_Exception_IO_lecture.ipynb) | 예외 전파와 처리, 사용자 정의 예외, 파일, CSV, JSON |
| 13 | [Pythonic Thinking & Design Patterns](L13_Pythonic_Patterns_lecture.ipynb) | 코드 관례, Decorator, 디자인 패턴, Type Hint, Docstring |

## 보충 자료

- [Control Flow 추가 예제](L05_control_flow_enhanced.ipynb): 조건 분기와 단락 평가, 멤버십 검색 비용을 비교하는 예제.
- [Class 1–6 복습](L08_review_class_1_6.ipynb): 앞에서 다룬 문법을 Namespace, Scope, Binding의 관점에서 다시 살펴보는 노트.
- [legacy](legacy/): 이전 버전의 강의 노트와 초기 작성 자료.

## 실습 방법

Jupyter Notebook이나 VS Code의 노트북 편집기에서 파일을 열고, 설명을 읽으며 셀을 위에서부터 실행한다. 앞선 셀에서 정의한 변수와 함수를 뒤에서 사용하므로, 실행 순서가 섞였다면 커널을 다시 시작하고 처음부터 실행한다.

`TODO`나 `pass`가 있는 실습 셀은 직접 구현한다. 실행 결과를 먼저 예상하고 실제 결과와 비교한 뒤, 노트 끝의 복습 질문으로 동작을 설명해 본다.
