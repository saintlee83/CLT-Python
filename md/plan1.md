🎓 Python 문법 체계 기반 심화 커리큘럼

핵심 목표: Python을 언어 구조, 실행 모델, 그리고 철학으로 이해한다.

⸻

I. 🧱 문법 구성요소 (Grammatical Components)

Python 코드의 “언어적 구성 요소”를 해부하는 단계

⸻

1. Lexical Structure — 어휘 단위와 토큰

학습 목표
• Python 소스가 토큰으로 분해되는 과정을 이해한다.
• Identifier, Keyword, Operator, Delimiter를 구분한다.
핵심 주제
• 토큰 유형: identifier / literal / operator / keyword
• 공백, 줄바꿈, 주석 처리 규칙
• Python의 어휘 분석기(lexer) 개념
실습
• tokenize 모듈을 사용해 코드의 토큰 구조 분석
• “Python 문장 해부” 실습 (for i in range(3): print(i))

⸻

2. Literal System — 값의 표현

학습 목표
• Python literal의 종류와 메모리 표현 방식을 이해한다.
핵심 주제
• 숫자형 (정수, 부동소수, 복소수, 진수 표현)
• 문자열 / bytes / f-string
• Boolean, None
• Collection literal: list, tuple, dict, set
실습
• 리터럴 → 객체 변환 (type, id)
• immutability 실험 (a = 10; b = 10; a is b)

⸻

3. Expression Elements — 표현식 구성

학습 목표
• 표현식과 문장의 구분을 명확히 이해한다.
핵심 주제
• 연산자 우선순위
• 함수 호출, 대입식 (:=)
• Short-circuit evaluation (and, or)
실습
• ast.parse()로 expression tree 시각화
• 식별자 해석 과정 trace하기 (dis.dis())

⸻

4. Statement Components — 문장의 구성

학습 목표
• Python statement의 구조와 종류를 이해한다.
핵심 주제
• Simple statements (import, return, pass, raise)
• Compound statements (if, for, try, with, def, class)
• 문장 종결 규칙 (세미콜론, 줄바꿈)
실습
• 여러 문장을 하나의 블록으로 파싱 → AST 출력

⸻

5. Object Model Basics — 객체의 본질

학습 목표
• “모든 것은 객체”라는 개념을 구체적으로 이해한다.
핵심 주제
• id, type, value 관계
• Mutability, Equality (is vs ==)
• Python Data Model의 개요
실습
• **eq**, **repr** 재정의로 객체 비교 실험

⸻

6. Function as Object — 함수의 일급 객체성

학습 목표
• 함수를 값으로 취급하는 Python 특성을 이해한다.
핵심 주제
• 일급 객체로서의 함수
• lambda, default argument, closure preview
• 함수 객체의 속성 (**name**, **doc**)
실습
• 함수 리스트 관리, 고차함수 체험 (map, filter, sorted(key=))

⸻

II. ⚙️ 문법의 구조 (Grammatical Structures)

문법 요소들이 결합되어 의미를 만드는 방식 이해

⸻

7. Control & Flow Structure — 제어문

학습 목표
• 조건 분기와 반복의 구조를 문법적으로 이해한다.
핵심 주제
• if, elif, else
• for, while, break, continue, else
• Truthy / Falsy 평가
실습
• 조건문 트리 시각화, 루프 내부 흐름 trace

⸻

8. Iteration Protocol — 반복의 내부 구조

학습 목표
• Iterable과 Iterator의 동작 원리를 이해한다.
핵심 주제
• **iter**, **next**
• for문 내부에서 iterator 소비
• Generator 함수 (yield)
실습
• custom iterator 클래스 만들기
• generator vs list 비교 (sys.getsizeof)

⸻

9. Comprehension & Context Manager

학습 목표
• comprehension 문법과 context 관리 구조를 익힌다.
핵심 주제
• list/dict/set comprehension
• generator expression
• with문과 **enter**, **exit**
실습
• context manager 직접 구현 (class File: …)

⸻

10. Block & Indentation Structure

학습 목표
• 들여쓰기가 문법적 구조로 작동하는 원리를 이해한다.
핵심 주제
• Block 구조, Scope 형성, Nesting
• Control Structure 안의 문맥(Context)
실습
• 중첩 if/for 구조의 코드 블록 추적
• ast.dump()로 구조 비교

⸻

11. Function & Abstraction Structure

학습 목표
• 함수 정의, 클로저, 데코레이터 구조 이해
핵심 주제
• def, lambda, default / keyword / variadic args
• closure, nonlocal
• decorator (함수를 반환하는 함수)
실습
• @timer, @logger 데코레이터 구현

⸻

12. Module & Package Structure

학습 목표
• import 시스템과 모듈 네임스페이스 이해
핵심 주제
• import, **name**, sys.modules
• 절대/상대 import
• 패키지 구조와 **init**.py
실습
• 간단한 3파일 패키지 구성 → import trace

⸻

III. 🧩 실행 모델 (Execution Model & Internals)

⸻

13. Namespace & Scope System

학습 목표
• Python의 이름 해석 규칙(LEGB)을 실험적으로 이해한다.
핵심 주제
• Local, Enclosing, Global, Built-in
• globals(), locals()
• global, nonlocal 키워드
실습
• 클로저 내부 변수 shadowing 실험

⸻

14. Execution Frame & Call Stack

학습 목표
• 함수 호출 시 생성되는 프레임과 실행 컨텍스트를 이해한다.
핵심 주제
• Frame, Stack, Code object
• inspect 모듈, call stack tracing
실습
• 함수 호출 중 stack frame 출력하기

⸻

15. Memory & Garbage Collection

학습 목표
• 객체의 생명주기와 메모리 관리 원리를 학습한다.
핵심 주제
• Reference Counting
• Garbage Collector (gc 모듈)
• weakref를 이용한 순환 참조 해결
실습
• 참조 그래프 시각화 (object reference map)

⸻

16. Bytecode & Interpreter

학습 목표
• Python 코드가 Bytecode로 변환되고 실행되는 과정을 이해한다.
핵심 주제
• 컴파일 → Bytecode → 실행
• dis 모듈로 opcode 분석
실습
• dis.dis(func)로 함수 실행 흐름 분석

⸻

17. GIL & Concurrency

학습 목표
• Python의 GIL 개념과 병렬성 한계를 이해한다.
핵심 주제
• Thread vs Process
• GIL의 동작 원리
• threading, multiprocessing 비교
실습
• CPU-bound vs I/O-bound 성능 비교 실험

⸻

18. Async & Coroutine Model

학습 목표
• 비동기 프로그래밍의 문법과 이벤트 루프 이해
핵심 주제
• async def, await, asyncio
• coroutine 개념, task scheduling
실습
• 간단한 async downloader 작성

⸻

IV. 🧠 언어적 사고 (Pythonic Thinking & Philosophy)

⸻

19. Pythonic Idioms

학습 목표
• Pythonic 스타일의 코드를 습득한다.
핵심 주제
• EAFP vs LBYL
• Duck Typing
• Comprehension, unpacking, chaining
실습
• “비Pythonic 코드”를 “Pythonic하게” 리팩터링

⸻

20. Decorator & Metaprogramming

학습 목표
• 런타임 코드 조립과 동적 클래스 생성 이해
핵심 주제
• Function/Class Decorator
• type()을 이용한 클래스 동적 생성
• 메타클래스 (**new**, **init_subclass**)
실습
• 메타클래스로 Singleton 구현

⸻

21. Descriptor & Property

학습 목표
• 속성 제어 프로토콜의 원리 이해
핵심 주제
• **get**, **set**, **delete**
• property() 함수와 데코레이터 비교
실습
• 데이터 검증용 descriptor 작성

⸻

22. Dataclass & Type Hinting

학습 목표
• 정적 분석과 구조화 데이터 선언 학습
핵심 주제
• @dataclass
• Typing (List, Dict, Optional)
• Pydantic-style validation 개념
실습
• dataclass 기반 설정 객체 설계

⸻

23. Design Patterns in Python

학습 목표
• Python의 문법적 특성을 활용한 설계 패턴 이해
핵심 주제
• Singleton, Factory, Observer, Context
• 함수형 패턴 (partial, closure 기반)
실습
• Strategy 패턴을 데코레이터로 구현

⸻

24. Python Philosophy

학습 목표
• Python의 언어 철학을 이해하고 코드 스타일에 적용한다.
핵심 주제
• Zen of Python (import this)
• “Simple is better than complex” 철학
• Guido van Rossum의 디자인 원리
실습
• 철학적 원칙을 반영한 코드 리뷰 실습

⸻

📚 전체 요약 구조

구분 학습 초점 주요 키워드 학습 성과
문법 구성요소 언어의 기본 단위 Token, Literal, Object, Function 언어 해석의 기초
문법의 구조 문장과 제어 구조 Control, Block, Module 문법적 구조 설계 능력
실행 모델 내부 실행 원리 Scope, Frame, GC, Bytecode 인터프리터 동작 이해
언어적 사고 언어의 철학과 메타 구조 Decorator, Duck Typing, Zen Pythonic 사고 정립

⸻

📘 결론:
이 커리큘럼은 “프로그래밍 언어로서의 Python”을 완전히 이해하기 위한 언어학적·공학적 통합 과정입니다.
즉, 단순히 “파이썬 개발자”가 아닌

“Python 언어의 원리를 설계 수준에서 이해하는 엔지니어”
로 성장하는 로드맵이에요.

⸻

원하신다면 🎓 15주 강의계획서형 (Week 1~15) 로 재구성해서
• 학습 목표
• 이론 주제
• 실습 과제
• 평가 포인트

까지 포함된 완전한 syllabus 버전으로 만들어드릴까요?
