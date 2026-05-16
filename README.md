# Claude Code 소스 코드 Deep Dive

Claude Code의 내부 아키텍처를 소스 코드 관점에서 분석하는 한국어 학습 사이트입니다. 부팅 시퀀스, 도구 시스템, 에이전트 실행, 권한, 메모리, UI, 인프라, MCP, SDK, 미공개 기능까지 구조적으로 정리합니다.

## 대상

- Claude Code가 실제로 어떻게 부팅되고 에이전틱 루프를 실행하는지 알고 싶은 개발자
- 도구 호출, 권한, 메모리, 컨텍스트 조립, UI 렌더링 구조를 코드 수준에서 이해하려는 사용자
- 코딩 에이전트나 개발자 도구를 직접 설계하려는 엔지니어

## 구성

- 10개 섹션
- 51개 MDX 챕터
- 10개 섹션별 퀴즈
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
10. 미공개 기능과 전체 조망: model system, BUDDY, KAIROS, ULTRAPLAN, desktop entrypoints, synthesis

## 로컬 개발

```bash
pnpm install
pnpm dev
pnpm build
pnpm preview
```

## 주요 경로

- 문서 본문: `src/content/docs/`
- 퀴즈 데이터: `public/data/quiz/`
- 공통 학습 컴포넌트: `src/components/learning/`
- 스타일: `src/styles/`
- 사이트 설정: `astro.config.mjs`
