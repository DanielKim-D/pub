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
llama model download --source meta --model-id  MODEL_ID

## 사용자 정의 URL을 지정하세요
라마 3.1: 405B, 70B & 8B
스크립트에서 고유한 사용자 지정 URL을 요청하면 아래 URL을 붙여넣으세요.
웹 주소
https://llama3-1.llamameta.net/*?Policy=eyJTdGF0ZW1lbnQiOlt7InVuaXF1ZV9oYXNoIjoiYjk0MXZ0YnExd29taXJuOHIyMXV5N29vIiwiUmVzb3VyY2UiOiJodHRwczpcL1wvbGxhbWEzLTEubGxhbWFtZXRhLm5ldFwvKiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTczMTc0MDc4N319fV19&Signature=TFq7D1yv46gQbfrkdZA0etcZQafEZHpJukkP5XGtBVeGJ9GV8K6BY5sVDrdyw8-KxMg4mZ0Q2p%7EfMFaxNyiEUQ9d4-fnq-T3LwnjFzHxxu%7E%7EG%7EtBE6U3apdEerKbSxxEkMlluDBlvP1k%7E3mHJfVB-ZrUwL4lbadYYAY84evKms5uJb-HOhgDcxvWJ5hciufvD%7Ev1-7goE-vg5UkLLksCRpt1YK9KB5rfDoKQe04fmclZUZPV--Pz5mNb-nGof6w73lOw4PsYC17mNS99KpmPCSW0kKnPgLLgK2d1livMNmaJTP3oe5HMFha5RukDvkGdD4pG5IjCtwmuSFAIqKKhEQ__&Key-Pair-Id=K15QRJLYKIFSLZ&Download-Request-ID=533635576234184
위에 제공된 고유한 사용자 지정 URL의 사본을 저장하세요. 이 URL은 각 모델을 최대 5회까지 다운로드할 수 있는 48시간 동안 유효하며 , 요청은 여러 번 제출할 수 있습니다. 다운로드 지침이 포함된 이메일도 모델을 요청하는 데 사용한 이메일 주소로 전송됩니다.
