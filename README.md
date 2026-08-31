# AI Quality Engineer / Senior QA Engineer Portfolio

> LLM·Agent 기반 서비스의 **출력 품질(할루시네이션·응답 정합성)**, **Agent 수행 결과**, 그리고 **릴리즈 Quality Gate**를 검증하는 QA 포트폴리오입니다.
> 핵심은 자동화 코드 자체가 아니라 **리스크 식별, 테스트 설계, 증거 수집, 릴리즈 판단**입니다.

<p align="center">
  <img src="assets/profile.png" alt="훌륭한 AI QA는 기술 역량, 분석 역량, 호기심, 문서 커뮤니케이션, AI QA 전문 역량, 생산성, 태도의 조합으로 만들어진다는 설명 이미지" width="680">
</p>

---

## 저는 이런 QA 엔지니어입니다

저는 테스트를 단순히 정해진 케이스를 수행하는 일이 아니라,
**요구사항과 구현 사이의 리스크를 발견하고 릴리즈 판단에 필요한 근거를 만드는 일**이라고 생각합니다.

2015년부터 QA 엔지니어로 일하며 요구사항 검토, 테스트 전략 수립, 결함 분석, 회귀 범위 선정, 릴리즈 판단을 중심으로 경험을 쌓아왔습니다.
최근에는 AI 제품이 늘어나면서 **"AI를 QA에 활용하는 것"을 넘어 "AI 제품의 출력과 수행 결과 자체를 검증하는 것"**이 QA의 새로운 핵심이라고 보고, 그 문제의식을 실제 코드와 파이프라인으로 정리했습니다.

제가 중요하게 보는 QA의 역할은 다음과 같습니다.

- 모든 것을 테스트하려 하기보다, 가장 위험한 영역을 먼저 찾는 것
- 단순 PASS / FAIL 보고보다, 남은 리스크를 설명하는 것
- 자동화를 많이 만드는 것보다, 자동화할 대상을 올바르게 고르는 것
- AI 결과를 그대로 믿기보다, 검증 가능한 기준 안에서 활용하고 그 품질을 정량 평가하는 것
- 최종적으로 "이번 릴리즈가 나가도 되는가?"에 대해 근거 있게 말하는 것

한 줄로 요약하면,
**저는 테스트 실행보다 리스크 판단과 품질 의사결정을 더 중요하게 보는 QA 엔지니어입니다.**

---

## 포트폴리오 안내

이 포트폴리오의 데이터, 식별자, 기준값, 시나리오, 화면, 로그는 모두 공개 데모 사이트 또는 직접 생성한 가상 데이터입니다. 현재 또는 과거 회사/고객사의 운영 데이터, 내부 문서, 비공개 명세, 실제 서비스 정보는 포함하지 않습니다.

---

## 포지셔닝

| 영역         | 요약                                                                                |
| ------------ | ----------------------------------------------------------------------------------- |
| 직무 방향    | AI Quality Engineer / Senior QA Engineer                                            |
| 경험         | 2015년부터 QA 엔지니어로 일해왔습니다 (10년+)                                       |
| 핵심 강점    | 요구사항 검토, 테스트 전략, 회귀 범위 선정, 결함 분석, 릴리즈 게이트 운영           |
| AI 특화      | LLM 출력 평가(DeepEval), Agent 수행 결과 검증, 도메인 특화 평가셋 구축              |
| 테스트 관점  | 버그 탐색보다 리스크 식별, 영향 분석, 의사결정 근거 수집을 중시합니다               |
| 자동화 관점  | 자동화는 목적이 아니라 회귀 리스크와 운영 부담을 줄이기 위한 지원 도구입니다        |
| AI 활용 관점 | AI에게 QA를 맡기는 것이 아니라, AI가 만든 결과를 검증 가능한 구조 안에서 활용합니다 |

---

## 대표 프로젝트

| 프로젝트 | QA 역량 | 핵심 메시지 | 핵심 기술 스택 |
| --- | --- | --- | --- |
| [`botserver`](https://github.com/tempesty-ai/botserver) | 사내 챗봇 구축·운영 | 반복 질문과 인터럽트 비용을 줄이는 QA 지원 챗봇을 기획·설계·구현 단독 주도 후 팀에 운영했습니다. 커넥터가 질문에 맞는 사내 문서를 검색해 첨부하는 RAG 구조로, 답변이 문서 근거를 갖도록 했습니다 | `Flask` `OpenAI Assistant API` `RAG (file_search / vector store)` `Mattermost` |
| [`ttalkkak-bug-reporter`](https://github.com/tempesty-ai/ttalkkak-bug-reporter) 🏆 | AI 결함 리포팅 자동화 (사내 공모전 수상) | 로컬 AI가 메모·콘솔 에러·스크린샷을 종합해 리포트를 정형화하고, 버그 발견부터 등록까지를 30초로 줄입니다 | `Ollama` `Chrome MV3` `ClickUp API` `Vanilla JS` |
| [`UI_Test`](https://github.com/tempesty-ai/UI_Test) | AI 에이전트 검증 | AI 에이전트를 그대로 믿지 않고 하네스로 통제하며, 그 수행 결과를 사람이 재검증해 신뢰도를 지표화합니다 | `Playwright MCP` `Claude Code Hooks` `Python` `Cron` |
| [`aiops-sentinel`](https://github.com/tempesty-ai/aiops-sentinel) | AI 출력 품질 평가 | AI가 생성한 장애 분석 결과를 DeepEval 기준으로 환각·정합성까지 다시 평가합니다 | `Python` `DeepEval` `LangChain` `Ollama` |
| [`qa-release-gate`](https://github.com/tempesty-ai/qa-release-gate) | 릴리즈 리스크 판단 | 테스트 결과·결함·변경 범위·rollback 준비도를 종합해 GO / CONDITIONAL_GO / NO_GO를 판단하고 CI에 연동합니다 | `Python` `Streamlit` `GitHub Actions` `pytest` |
| [`apm-qa-automation`](https://github.com/tempesty-ai/apm-qa-automation) | 비기능(성능) 자동화 | 기능 검증과 부하 테스트를 하나의 파이프라인에 묶어 CI에서 자동 실행합니다 | `pytest` `Locust` `Docker Compose` `GitHub Actions` |
| [`ui-harness`](https://github.com/tempesty-ai/ui-harness) | UI 회귀 자동화 | 반복 회귀 리스크가 큰 핵심 플로우를 선별해 자동화합니다 | `Selenium` `Playwright` `pytest` `Page Object` |

## 포트폴리오 스토리라인

대표 프로젝트 표와 같은 순서입니다. 각 항목은 그 프로젝트가 답하려는 질문입니다.

```text
botserver
  -> QA가 반복적으로 받는 장애/성능/배포 질문을 사내 문서 근거와 함께 챗봇으로 1차 대응

ttalkkak-bug-reporter
  -> 발견한 결함을 사람이 다시 정리하지 않도록, 로컬 AI가 증거와 함께 리포트로 정형화

UI_Test
  -> 일반 자동화로 놓치기 쉬운 시각적 회귀를 AI 에이전트와 하네스로 점검하고 결과를 재검증

aiops-sentinel
  -> AI가 만든 장애 분석 결과를 운영에 써도 되는지 품질 기준으로 정량 평가

qa-release-gate
  -> 이번 릴리즈가 나가도 되는지 설명 가능한 기준으로 판단

apm-qa-automation
  -> 부하 조건에서의 성능 회귀까지 CI에서 자동 확인

ui-harness
  -> 반복 회귀를 줄이기 위해 무엇을 자동화할지 리스크 기준으로 선별
```

공통 질문은 다음과 같습니다.

> 도구와 AI가 실제로 회귀 리스크를 줄이는가?
> 그리고 그 결과를 어떤 기준으로 신뢰하고 릴리즈 판단에 연결할 수 있는가?

---

## 프로젝트별 평가 포인트

| 프로젝트                     | 문제 상황                                                                                   | 제가 보여주려는 판단                                                                    |
| ---------------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `botserver`                | QA가 반복 질문에 계속 응답하면 컨텍스트 스위칭 비용이 커지고, 근거 없는 답변은 오히려 재확인 비용을 만듦 | 협업 도구 안에서 QA 지식을 1차 응답 가능하게 구조화하되, RAG로 사내 문서를 근거로 붙여야 신뢰할 수 있음 |
| `ttalkkak-bug-reporter` | 결함 리포트 작성 부담이 크면 재현 절차와 증거가 누락된 채 등록됨 | 증거 수집을 자동화해야 리포트 품질이 사람의 컨디션에 좌우되지 않음 |
| `UI_Test`                  | HTTP 200이나 일반 E2E 통과만으로는 레이아웃 깨짐, 요소 겹침, 모바일 화면 문제를 잡기 어려움 | AI 에이전트는 자율 실행보다 통제 가능한 하네스 안에서 활용하고, 그 판정을 재검증해야 함 |
| `aiops-sentinel`           | AI가 생성한 장애 분석은 그럴듯하지만 실제 운영 판단에 바로 쓰기에는 위험할 수 있음          | AI 출력도 hallucination, relevance, faithfulness 관점에서 검증해야 함                   |
| `qa-release-gate`          | 테스트 통과율만으로 배포 여부를 판단하면 중요 결함과 rollback 리스크가 누락될 수 있음       | 릴리즈 판단은 pass/fail이 아니라 남은 리스크와 준비 상태를 종합해야 함                  |
| `apm-qa-automation` | 기능 테스트만 통과해도 부하 조건에서 응답 지연이나 실패가 발생할 수 있음 | 비기능 품질은 릴리즈 직전 수동 확인이 아니라 CI에서 상시 측정되어야 함 |
| `ui-harness`               | 반복 회귀를 사람이 매번 확인하면 누락과 피로도가 커짐                                       | 자동화 대상은 반복 빈도, 실패 영향도, 결과 명확성 기준으로 선별해야 함                  |

---

## 릴리즈 판단 기준

릴리즈 판단은 단순 테스트 통과율만으로 결정하지 않습니다.

- Critical / Blocker 결함 존재 여부
- P1/P2 미해결 결함과 사용자 영향
- 변경 범위가 로그인, 결제, 권한, 데이터 처리 등 critical area인지 여부
- 핵심 사용자 플로우 회귀 테스트 통과 여부
- 자동화 커버리지와 수동 보강 테스트 필요 여부
- rollback plan 존재 여부 / rollback test 수행 여부
- 배포 후 monitoring owner 지정 여부

| 판단           | 의미                                                                          |
| -------------- | ----------------------------------------------------------------------------- |
| GO             | 핵심 리스크가 통제되고 배포 후 감시와 rollback 준비가 완료된 상태             |
| CONDITIONAL_GO | 일부 리스크는 남아 있으나 우회 방안, 비즈니스 승인, 모니터링 조건이 있는 상태 |
| NO_GO          | 사용자 영향이 큰 결함 또는 복구 준비 부족으로 배포를 막아야 하는 상태         |

---

## 기술 스택

**언어 · 자동화** Python · pytest · Selenium · Playwright · JavaScript · Postman
**비기능 · 부하** Locust · Docker Compose
**AI · LLM 품질 평가** DeepEval · LangChain · Ollama · Playwright MCP · Claude Code Hooks · OpenAI Assistant API
**플랫폼 · 운영** GitHub Actions (CI/CD) · Flask · Streamlit · Mattermost · Chrome Extension (MV3)

---

## Portfolio Summary

이 포트폴리오는 QA 업무를 단순 테스트 실행이 아니라, **리스크 식별, 검증 설계, 자동화 활용, AI 출력 품질 평가, 릴리즈 판단**으로 확장해 보는 실험입니다.

핵심 메시지는 "자동화를 할 수 있다"가 아니라, **자동화와 AI 결과를 품질 판단과 릴리즈 의사결정에 연결할 수 있다**는 점입니다.

---

## 연락처
- 👤 김영신 (Kim Young Shin)
- 📧 tempesty7207@gmail.com
- 💻 github.com/tempesty-ai
