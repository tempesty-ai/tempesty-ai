# QA Engineer / PMO Portfolio

> A QA/PMO portfolio showing how quality work can be redesigned with AI-assisted tools.

## Portfolio Disclaimer

All data, identifiers, thresholds, scenarios, screens, and logs in these repositories are based on public demo sites or self-generated virtual data. They do not include production system information, operational data, internal documents, or private specifications from any current or former company or customer.

## Positioning

| Area | Summary |
| --- | --- |
| Experience | QA engineer since 2009, currently also working with PMO responsibilities |
| Strengths | Requirements review, test strategy, regression scope, defect analysis, release gate operation |
| Interest | Redesigning QA work in the AI era with LLM and agent-oriented tools |
| Automation view | Automation is a support tool for reducing regression risk and operational load, not the goal itself |

## Portfolio Structure

These repositories answer one shared question:

> When QA adopts LLMs and AI agents as tools, how does day-to-day quality work change?

| # | Repository | QA Area | Technologies |
| --- | --- | --- | --- |
| 1 | [`ok`](https://github.com/tempesty-ai/ok) | UI regression automation foundation | Selenium, Playwright, pytest |
| 2 | [`UI_Test`](https://github.com/tempesty-ai/UI_Test) | Visual QA execution pipeline | Playwright MCP, Claude Code Hook |
| 3 | [`botserver`](https://github.com/tempesty-ai/botserver) | QA support chatbot for collaboration tools | Flask, OpenAI Assistant API, Mattermost |
| 4 | [`aiops-sentinel`](https://github.com/tempesty-ai/aiops-sentinel) | AIOps monitoring and AI output quality evaluation | LangChain, Ollama, DeepEval |

## How The Repositories Connect

```text
ok
  -> choose what should be automated
UI_Test
  -> delegate repeatable visual inspection to a controlled pipeline
botserver
  -> expose QA knowledge through a chat interface
aiops-sentinel
  -> evaluate whether AI-generated analysis can be trusted
```

The common QA question is: does the tool actually reduce regression risk, and how can that be measured?

## Suggested Entry Points

| Interest | Start With |
| --- | --- |
| Traditional QA automation | `ok` |
| AI-assisted visual QA | `UI_Test` |
| Collaboration and chatbot integration | `botserver` |
| LLM output quality evaluation | `aiops-sentinel` |

## Current Roadmap

- Add before/after measurements to each repository README
- Add measured DeepEval results to `aiops-sentinel`
- Align disclaimers and contribution notes across repositories
- Prepare a slide deck version of the portfolio story