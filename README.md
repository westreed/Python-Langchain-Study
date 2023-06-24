# Python Langchain Study

## Install

```commandline
pip install langchain
pip install openai                  // ChatGPT API
pip install google-search-results   // Google Search API
```

## Learning

1. 언어모델(LLMs)

텍스트 문자열을 입력하고, 텍스트 문자열을 출력하는 모델입니다.
LangChain 은 LLM 공급자가 아니며, 인터페이스만 제공합니다.  
`언어모델은 OpenAI의 text-davinci-003 모델을 사용함.`

2. 채팅모델(Chat)

채팅 모델은 언어 모델의 변형으로, 내부적으로는 언어 모델을 사용하지만 노출되는 인터페이스는 약간 다릅니다.
현재는 System, Human, AI 3종류의 사용자를 지원합니다.  
`언어모델은 OpenAI의 Chat-gpt-3.5-turbo 모델을 사용함.`

- System : AI에게 해야 할 일을 알려주는 배경 컨텍스트
- Human : 사용자 메세지
- AI : AI가 응답한 내용을 보여주는 상세 메세지

3. Memory

기본적으로 Chain 및 Agent는 `Stateless`입니다.
즉, 기본 LLM 및 채팅 모델과 같이 입력받은 각 쿼리를 독립적으로 처리합니다.
챗봇과 같은 일부 앱에서는 대화를 기억하는 기능이 필요하고, Memory가 해당 기능을 수행합니다.

- ConversationChain의 경우에는 AI Message가 자동으로 기입됨.
- 초기질문을 생성하고 질문을 하면 사용자는 답변하는 구조인데,
질문은 이미 생성되었기 때문에 질답이 끝나면 다음 질문 텍스트를 넣어줘야함.
- ConversationChain의 경우에는 사용자가 먼저 메시지를 보내면, AI가 응답하는데 이 응답이 강제적으로 기록됨.
- 




## ETC

PyCharm 커뮤니티버전에서 쥬피터 노트북을 쓰고 싶을 땐,
[링크](https://tariat.tistory.com/169) 참고하세요.