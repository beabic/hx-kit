# hx-kit

Codex 로 해커톤 과제를 풀 때 쓰는 작업 규칙 스킬 `hx` 하나.

- 만든 사람: [beabic](https://github.com/beabic) · 2026-10-30
- 용도: SK하이닉스 AI 해커톤 2026 2차 예선(Cofa-Probe) 응시 환경에서 내가 쓰려고 미리 만들어 공개했다. **과제 답이나 과제용 코드는 들어 있지 않다** — 일하는 순서와 지킬 규칙만 있다.
- 시험 때 쓰는 판은 이 커밋(태그 `exam`)이다. 2차 예선 결과가 나올 때까지 공개로 두고 고치지 않는다.

## 쓰는 법

과제 폴더에서:

```sh
git clone -q --depth 1 https://github.com/beabic/hx-kit .agents/skills/hx
rm -rf .agents/skills/hx/.git
```

그다음 Codex 에서 `$hx 시작` → `$hx 나누기` → `$hx 기록 …` → `$hx 설계` → `$hx 카드 C1` …

## 모드

| 언제 | 부르는 말 | 하는 일 |
|---|---|---|
| 처음 | `$hx 시작` | git 준비 · `.gitignore`(비밀값 맨 위) · 런타임 확인 · `AGENTS.md` 3줄 · `PLANS.md` 틀 |
| README 읽고 | `$hx 나누기` | README 를 7칸 표로 `.hx/interview.md` 에 (README 는 그대로) · 첫 질문 후보 3개 |
| 담당자 답마다 | `$hx 기록` | 질문 / 답 원문 / 요약 / 바뀐 결정 |
| 설계 | `$hx 설계` | 가장 작은 안 + 대안 하나 → `.hx/decisions.md` |
| 구현 | `$hx 카드 N` | 5줄 계획만 → 승인 뒤 그 범위만 구현·테스트 |
| 맡기기 | `$hx 위임 N` | 서브에이전트 하나에 |
| 커밋마다 | `$hx 커밋` | 바뀐 파일·비밀값 검사 → add 목록과 메시지만 제안(실행은 사람) |
| 90분 | `$hx 점검` | 화면 흐름 · 테스트 · README 실행 · git 상태 |
| 마무리 | `$hx 마무리` | README 를 실제 코드대로 · 필수 파일·비밀값 확인 |
| 서술형 전 | `$hx 복습` | 내 코드 기준 숫자 다섯 · 예상 질문 6 |
| 길어지면 | `$hx 인계` | `.hx/handoff.md` |

## 원칙

판단과 확인은 사람이, 실행은 Codex 가. 합의 전에 만들지 않고, 들은 것만 기록하고, 비밀값은 열지 않고, 커밋은 사람이 한다.

MIT License.
