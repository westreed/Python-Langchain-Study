# 유즈케이스

[CreateQuestion]
- DataManager에 저장된 사용자 정보를 입력받는다.
- 질문을 생성하기 위한 프롬프트를 생성한다.
- 프롬프트를 생성할 때 사용자 정보를 추가한다.
- 질문 생성 프롬프트를 통해 LLMChain을 만든다.
- Chain에 입력(생성할 질문 갯수)을 받는다.
- 해당 입력에 대한 Chain을 적용한다.
- 출력으로 N개의 질문이 생성된다.
  - 생성된 질문은 create_question_parser를 통해 List형태로 만든다.
- 파싱한 질문리스트를 반환한다.

![시퀀스다이어그램](https://github.com/westreed/Python-Langchain-Study/raw/main/mvp/img/CreateQuestionDiagram.png)