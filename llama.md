## Llama CLI 설치

원하는 환경에서 아래 명령을 실행하세요.
명령 pip install llama-stack
이전 버전이 이미 설치되어 있는 경우 -U 옵션을 사용하여 llama-stack을 업데이트하세요.
명령 pip install llama-stack -U

## 모델 목록 찾기

다음 명령을 실행하여 최신 사용 가능한 모델을 확인하고 다운로드하려는 모델 ID를 확인하세요.
명령 llama model list
이전 버전의 모델이 필요한 경우 아래 명령을 실행하여 사용 가능한 모든 Llama 모델을 표시하세요.
명령 llama model list --show-all

## 모델을 선택하세요

다음을 실행하여 원하는 모델을 선택하세요.
명령
llama model download --source meta --model-id MODEL_ID

## 사용자 정의 URL을 지정하세요

라마 3.1: 405B, 70B & 8B
스크립트에서 고유한 사용자 지정 URL을 요청하면 아래 URL을 붙여넣으세요.
웹 주소
https://llama3-1.llamameta.net/*?Policy=eyJTdGF0ZW1lbnQiOlt7InVuaXF1ZV9oYXNoIjoiYjk0MXZ0YnExd29taXJuOHIyMXV5N29vIiwiUmVzb3VyY2UiOiJodHRwczpcL1wvbGxhbWEzLTEubGxhbWFtZXRhLm5ldFwvKiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTczMTc0MDc4N319fV19&Signature=TFq7D1yv46gQbfrkdZA0etcZQafEZHpJukkP5XGtBVeGJ9GV8K6BY5sVDrdyw8-KxMg4mZ0Q2p%7EfMFaxNyiEUQ9d4-fnq-T3LwnjFzHxxu%7E%7EG%7EtBE6U3apdEerKbSxxEkMlluDBlvP1k%7E3mHJfVB-ZrUwL4lbadYYAY84evKms5uJb-HOhgDcxvWJ5hciufvD%7Ev1-7goE-vg5UkLLksCRpt1YK9KB5rfDoKQe04fmclZUZPV--Pz5mNb-nGof6w73lOw4PsYC17mNS99KpmPCSW0kKnPgLLgK2d1livMNmaJTP3oe5HMFha5RukDvkGdD4pG5IjCtwmuSFAIqKKhEQ__&Key-Pair-Id=K15QRJLYKIFSLZ&Download-Request-ID=533635576234184

라마 3.2: 11B & 90B
스크립트에서 고유한 사용자 지정 URL을 요청하면 아래 URL을 붙여넣으세요.
웹 주소
https://llama3-2-multimodal.llamameta.net/*?Policy=eyJTdGF0ZW1lbnQiOlt7InVuaXF1ZV9oYXNoIjoiaWhnbzhxNWtvbGc0MGZmcTZicjhzMTlmIiwiUmVzb3VyY2UiOiJodHRwczpcL1wvbGxhbWEzLTItbXVsdGltb2RhbC5sbGFtYW1ldGEubmV0XC8qIiwiQ29uZGl0aW9uIjp7IkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNzMyMDg1MTAzfX19XX0_&Signature=O3zOpBa7vSt77o0bHCosb1BQcdQsHbySElpJJfTZ96-qjU5DwZ2xMRAqp35NdSTFn96LKnBp25A8HNQcy2LFha8Mcs8AMNWX--GpU5qT4MASggX7fxcgoPi0tE5C3XzwI%7E9wj-7kTW5B62%7EhhEYWTF4EKkhdsv8TiBh3isN65YYw2o2j-I1qH5iTN2B4lIAzZ02y1vldc4MxsGRnPECsOutaKunZKZe5dd6fTn1hN7%7Emop0dC7b8wV-eBw23agwvKPZnQ498R-zgSO0pQQsZFvuEvSvtxcVVWOfmH1JzSgb1soGCEmUupQj94WueyCVBqgAkxqQyegID900WcMsoRA__&Key-Pair-Id=K15QRJLYKIFSLZ&Download-Request-ID=984379170108140

위에 제공된 고유한 사용자 지정 URL의 사본을 저장하세요. 이 URL은 각 모델을 최대 5회까지 다운로드할 수 있는 48시간 동안 유효하며 , 요청은 여러 번 제출할 수 있습니다. 다운로드 지침이 포함된 이메일도 모델을 요청하는 데 사용한 이메일 주소로 전송됩니다.

## 확인

ollama list

## 다운/시작

ollama run llama3.1

Ollama는 인공지능(AI)과 자연어처리(NLP)의 분야에서 특정한 용어입니다. Ollama는 "Open-source Large Language Model"의
약자로, AI 연구자들의 공동 프로젝트로 시작된 오픈 소스 기반의 대형 언어 모델입니다.

**1. 개요**
Ollama는 2022년 초에 시작된 프로젝트로, 인공지능(AI)과 자연어처리(NLP)의 연구자들이 함께 참여하여 개발 중인 언어 모
델입니다. Ollama의 주요 목표는 사용자가 자신의 생각, 감정, 또는 경험을 표현하고 다른 사람과 공유할 수 있도록 하는 오
픈 소스 기반의 대형 언어 모델을 만드는 것입니다.

**2. 특징**

- **오픈 소스**: Ollama는 오픈 소스 프로젝트로, 누구든지 코드를 가져와 자신이 원하는 방식으로 사용하거나 개선할 수
  있습니다.
- **대형 언어 모델**: Ollama는 대형 언어 모델로, 이전의 언어 모델에 비해 훨씬 더 많은 데이터와 복잡한 구조를 가지고
  있습니다. 이로 인해 Ollama는 다양한 자연어 처리 작업을 수행하고 더 정확한 결과를 내놓습니다.
- **다양한 용도**: Ollama는 다양한 용도로 사용할 수 있습니다. 예를 들어, 챗봇, 언어翻訳, 텍스트 생성, 자연어처리 및
  기타 AI 관련 작업에서 활용할 수 있습니다.

**3. 주요 기능**

- **자연어 처리**: Ollama는 자연어 처리 작업을 수행하고 다양한 텍스트 분석을 할 수 있습니다.
- **텍스트 생성**: Ollama는 사용자가 원하는 방식으로 텍스트를 생성할 수 있습니다.
- **인터랙션**: Ollama는 사용자와 대화를 나눌 수 있으며, 사용자의 입장과 시각을 이해할 수 있습니다.

**4. 개발 과정**
Ollama의 개발은 공동 작업 공간에서 진행되고 있습니다. 이 프로젝트에는 많은 AI 연구자와 개발자가 참여하고 있습니다.
Ollama의 개발은 지속적이며, 새로운 기능 및 업데이트들이 계속하여 추가되고 있습니다.

**5. 잠재력과 가능성**

- **AI 분야 발전**: Ollama는 AI 분야에 큰 영향을 미칠 것으로 예상됩니다.
- **인공지능 교육**: Ollama는 인공지능(AI) 개발자와 연구자를 위해 유용한 훈련 데이터 및 테스트 환경을 제공할 것입니
  다.
- **소통 향상**: Ollama를 통해 사람들은 더 쉽게 소통하고 자신의 생각과 경험을 공유할 수 있습니다.

**6. 단점**

- **오픈 소스 프로젝트의 단점**: 오픈 소스 프로젝트는 보안 및 안정성에 대한 위험 요인 등이 있습니다.
- **개발의 난이도**: Ollama를 개발하는 것은 어렵고 시간과 노력을 많이드는 작업입니다.

**7. 향후 계획**
Ollama의 개발은 지속적으로 진행되고 있습니다. 향후, Ollama는 사용자 경험을 개선하고 다양한 기능을 추가하여 더 많은
사람들에게 도움이 될 것입니다.
