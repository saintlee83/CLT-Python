이 버전은 실제 전공 교과목 계획서로 바로 사용할 수 있는 수준으로,
주차별 이론 + 실습 + 학습목표 + 핵심 키워드까지 포함합니다.
강의 제목 예시:
「파이썬 문법 체계와 언어 구조 (Python Grammatical System & Language Structure)」

⸻

🎓 Python 문법 체계 기반 15주 강의계획서

📘 과목 개요

이 과목은 Python을 단순한 프로그래밍 도구가 아닌, 언어 체계로서 이해하도록 설계되었다.
Lexical → Syntax → Execution → Philosophy의 4단 구조를 통해,
Python의 문법적 구성요소, 구조적 관계, 실행 메커니즘, 언어 철학을 단계적으로 탐구한다.

⸻

📚 수업 목표
• Python 문법을 구성요소 단위로 해석하고 구조적 관계를 이해한다.
• 인터프리터 내부 동작(Execution Model, Scope, GC)을 실험적으로 이해한다.
• Pythonic 철학과 설계 원리를 기반으로 고급 언어 추상화를 구현한다.
• 실습을 통해 언어 내부 모델을 해석하고, Pythonic 코드 스타일을 습득한다.

⸻

📅 주차별 강의 계획

주차
주제
주요 내용
실습 / 과제
핵심 키워드

1주차
Python 언어 구조 개요
Python의 언어 철학, 인터프리터 구조, 문법 계층(Token → Expression → Statement → Block)
Python 실행 흐름 시각화 (dis, ast 예제)
Token, Interpreter, Grammar

2주차
Lexical Structure & Literal System
Token의 종류, Identifier, Keyword, Literal 유형과 표현
tokenize 모듈로 코드 파싱, 리터럴 타입 비교
Literal, Identifier, Tokenizer

3주차
Expression & Statement
표현식(값 계산 단위)과 문장(명령 단위) 구조, 연산자 우선순위
ast.dump()로 표현식 트리 출력, eval() 실험
Expression, Statement, AST

4주차
Object Model & Type System
Python의 객체 모델, type/value/id, mutable/immutable
id(), type() 비교, **eq** 오버라이딩
Object, Mutability, Dunder

5주차
Control Flow & Loop Structure
조건문과 반복문, 흐름 제어 (if, for, while, break, continue, else)
루프 내부 흐름 시각화, 조건문 트리 분석
Control Flow, Loop, Conditional

6주차
Iteration Protocol & Comprehension
Iterable / Iterator / Generator, comprehension 구조
Custom Iterator 클래스, generator memory 비교
**iter**, **next**, Comprehension

7주차
Function & Closure 구조
함수의 일급 객체성, 스코프, 클로저, 데코레이터 개요
nonlocal 예제, @timer 데코레이터 작성
Closure, Function Object

8주차
중간고사 (이론 + 코드 해석 실습)
AST 해석, for-loop 내부 구조, namespace 실험
문법 구조 해석 과제
—

9주차
Module & Package System
import 메커니즘, **name**, 패키지 구조, 모듈 캐싱
3파일 패키지 구성 및 모듈 추적 (sys.modules)
Import, Package, Namespace

10주차
Namespace & Scope Rule (LEGB)
Local, Enclosing, Global, Built-in, 변수 shadowing
globals(), locals(), closure 내부 변이 실험
Scope, LEGB, Variable Binding

11주차
Execution Frame & Memory Model
함수 호출 스택, Frame 객체, Garbage Collection
inspect.stack()으로 콜스택 출력, gc 실험
Frame, GC, Reference Counting

12주차
Bytecode & Interpreter Internals
Python 실행 흐름: Source → Bytecode → Execution
dis.dis()로 opcode 분석, bytecode tracing
Bytecode, PVM, Opcode

13주차
Concurrency & Async Model
GIL, Thread vs Process, Coroutine, asyncio
간단한 async downloader 제작
GIL, Threading, Async

14주차
Pythonic Thinking & Design Patterns
Duck Typing, EAFP, Decorator, Descriptor, Dataclass
Pythonic 코드 리팩토링 과제
Decorator, EAFP, Dataclass

15주차
언어 철학 & 기말 프로젝트 발표
Zen of Python, 언어 디자인 원리, 코드 리뷰 세션
미니언어 구현 or 언어 기능 확장 프로젝트
Zen of Python, Simplicity

⸻

🧠 학습 성과 평가 기준

평가 항목 비율 평가 내용
중간고사 25% 언어 구조 해석 및 코드 분석
기말 프로젝트 35% Python 내부 모델 구현 or 확장 실습
실습 및 과제 25% 주차별 실험 리포트 및 코드
참여 및 토론 15% 수업 중 코드 해석 및 철학 토론 참여

⸻

🧩 기말 프로젝트 제안 예시

주제 내용
🧱 Mini Python Parser ast 모듈을 이용해 간단한 파이썬 문법 해석기 제작
⚙️ Custom Iterator Engine **iter**, **next**를 이용한 데이터 스트림 구조 설계
🧠 Decorator Framework 데코레이터 체인을 활용한 플러그인 시스템
🔁 Async Task Runner asyncio 기반 간단한 event loop 구현
📦 Import Visualizer 모듈 import 경로 및 캐싱 시각화 도구 제작

⸻

📘 교재 및 참고 자료
• Fluent Python (Luciano Ramalho)
• Inside the Python Virtual Machine (Obie Fernandez)
• Python Language Reference (docs.python.org)
• Effective Python (Brett Slatkin)
• Zen of Python (import this)

⸻

💬 강의 요약 철학

“문법을 배운다” → “언어를 해석한다” → “언어를 설계한다.”

이 강의의 목표는 Python을 하나의 도구가 아닌,
**“문법적 사고와 추상화 구조를 가진 언어 시스템”**으로 바라보는 것이다.

수강 후에는
• Python 코드를 문법 트리(AST) 관점에서 해석할 수 있고,
• 함수/객체/모듈의 동작을 실행 프레임 수준에서 이해하며,
• Pythonic 철학을 실무 코드에 녹여낼 수 있게 된다.