# Claude Code 공개 기능 Deep Dive

Claude Code의 공개 문서와 CLI를 기준으로 도구 시스템, 에이전트 실행, 권한, 메모리, UI, MCP, Agent SDK를 구조적으로 학습하는 한국어 사이트입니다. 내부 구현으로 추정한 이름이나 문서화되지 않은 API는 사용법으로 다루지 않습니다.

## 대상

- Claude Code의 공개 기능과 안전한 작업 흐름을 이해하려는 개발자
- 도구 호출, 권한, 메모리, 컨텍스트, 확장 기능을 운영 관점에서 이해하려는 사용자
- 코딩 에이전트나 개발자 도구를 직접 설계하려는 엔지니어

## 구성

- 10개 섹션
- 50개 학습 챕터 + 홈 문서 1개
- 10개 섹션별 퀴즈 JSON 데이터
- Astro 6 + Starlight + React 기반

## 커리큘럼

1. 핵심 아키텍처: overview, boot sequence, agentic loop, query engine, state management
2. 도구 시스템: tool architecture, file tools, bash, search, web, extension
3. 에이전트 지능: subagent, multi-agent, coordinator mode, worktree isolation, prompts
4. 권한과 보안: permission architecture, rules, bash security, sandbox safety
5. 메모리와 컨텍스트: `CLAUDE.md`, context assembly, compaction, include rules, auto memory
6. 인터페이스와 UI: Ink renderer, interactive modes, commands, notifications, theme/keybindings
7. 인프라스트럭처: config, hooks, skills, sessions, plugins, error handling
8. 연결성과 확장: MCP overview/config, OAuth, Git integration, bridge/remote
9. SDK와 프로그래매틱 사용: SDK architecture, control protocol, TypeScript API, IDE/CI/CD
10. 공개 기능과 전체 조망: 모델 선택, agent teams, Plan mode, 공식 진입점, 운영 원칙

## 로컬 개발

```bash
pnpm install
pnpm dev
pnpm build
pnpm preview
```

## 검증

변경 후에는 다음 명령으로 Starlight 콘텐츠, MDX, React 컴포넌트, 정적 자산 경로를 확인합니다.

```bash
pnpm build
```

## 콘텐츠 품질 기준

- 기능 설명은 Anthropic의 공개 문서와 현재 CLI 레퍼런스를 우선합니다.
- 실험 기능은 공개 상태와 알려진 제한을 함께 적고, 문서화되지 않은 이름·플래그·패키지를 사용법으로 제시하지 않습니다.
- 도구, 권한, MCP, skills, hooks, Agent SDK 설명은 최소 권한·검증·감사 원칙과 함께 정리합니다.

## 주요 경로

- 문서 본문: `src/content/docs/`
- 퀴즈 데이터: `public/data/quiz/`
- 공통 학습 컴포넌트: `src/components/learning/`
- 스타일: `src/styles/`
- 사이트 설정: `astro.config.mjs`
