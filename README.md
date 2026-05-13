# QA Engineer 포트폴리오

> AI 도구를 활용해 QA 업무를 어떻게 다시 설계할 수 있는지 보여주는 QA 포트폴리오입니다.

<p align="center">
  <img src="assets/profile.png" alt="훌륭한 AI QA는 기술 역량, 분석 역량, 호기심, 문서 커뮤니케이션, AI QA 전문 역량, 생산성, 태도의 조합으로 만들어진다는 설명 이미지" width="680">
</p>

## 포트폴리오 안내

이 포트폴리오의 데이터, 식별자, 기준값, 시나리오, 화면, 로그는 모두 공개 데모 사이트 또는 직접 생성한 가상 데이터입니다. 현재 또는 과거 회사/고객사의 운영 데이터, 내부 문서, 비공개 명세, 실제 서비스 정보는 포함하지 않습니다.

## 포지셔닝

| 영역 | 요약 |
| --- | --- |
| 경험 | 2015년부터 QA 엔지니어로 일해왔습니다 |
| 강점 | 요구사항 검토, 테스트 전략, 회귀 범위 선정, 결함 분석, 릴리즈 게이트 운영 |
| 관심사 | LLM과 에이전트형 도구를 활용해 AI 시대의 QA 업무를 재설계하는 것 |
| 자동화 관점 | 자동화는 목적이 아니라 회귀 리스크와 운영 부담을 줄이기 위한 지원 도구입니다 |

## 포트폴리오 구성

이 저장소들은 하나의 공통 질문을 다룹니다.

> QA가 LLM과 AI 에이전트를 도구로 받아들일 때, 일상적인 품질 업무는 어떻게 달라질 수 있을까?

| # | 저장소 | QA 영역 | 기술 |
| --- | --- | --- | --- |
| 1 | [`ui-harness`](https://github.com/tempesty-ai/ui-harness) | UI 회귀 자동화 기반 | Selenium, Playwright, pytest |
| 2 | [`ui_test`](https://github.com/tempesty-ai/UI_Test) | 시각적 QA 실행 파이프라인 | Playwright MCP, Claude Code Hook |
| 3 | [`botserver`](https://github.com/tempesty-ai/botserver) | 협업 도구용 QA 지원 챗봇 | Flask, OpenAI Assistant API, Mattermost |
| 4 | [`aiops-sentinel`](https://github.com/tempesty-ai/aiops-sentinel) | AIOps 모니터링과 AI 출력 품질 평가 | LangChain, Ollama, DeepEval |
| 5 | [`qa-release-gate`](https://github.com/tempesty-ai/qa-release-gate) | 릴리즈 리스크 판단과 QA 의사결정 | Python, Streamlit, pytest |

## 저장소 연결 흐름

```text
ui-harness
  -> 무엇을 자동화할지 선택
ui_test
  -> 반복 가능한 시각 검사를 통제된 파이프라인에 위임
botserver
  -> QA 지식을 채팅 인터페이스로 노출
aiops-sentinel
  -> AI가 생성한 분석을 신뢰할 수 있는지 평가
qa-release-gate
  -> 릴리즈를 진행해도 되는지 리스크 기반으로 판단
```

공통 QA 질문은 이것입니다. 도구가 실제로 회귀 리스크를 줄이는가, 그리고 그것을 어떻게 측정할 수 있는가?

## 추천 시작점

| 관심 영역 | 먼저 볼 저장소 |
| --- | --- |
| 전통적인 QA 자동화 | `ui-harness` |
| AI 보조 시각적 QA | `ui_test` |
| 협업 도구와 챗봇 연동 | `botserver` |
| LLM 출력 품질 평가 | `aiops-sentinel` |
| 릴리즈 판단과 QA 리드 관점 | `qa-release-gate` |

## 현재 로드맵

- 각 저장소 README에 전후 비교 측정값 추가
- `aiops-sentinel`에 측정된 DeepEval 결과 추가
- 저장소별 안내 문구와 기여 메모 정렬
- 포트폴리오 스토리의 발표 자료 버전 준비
