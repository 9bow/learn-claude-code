# 추가 용어

이 문서는 [terms.kr 용어 데이터](https://poc.terms.kr/llms.txt)를 확인했을 때 수록되지 않은, 이 학습 사이트에서 필요한 Claude Code 관련 용어만 정의합니다. 일반 용어인 에이전트(agent)는 terms.kr의 기존 용어를 따릅니다. 기능의 사용 가능 여부와 세부 옵션은 각 공식 문서를 기준으로 확인합니다.

| 용어 | 한국어 표기 | 정의 | 공식 근거 |
| --- | --- | --- | --- |
| Agent SDK | 에이전트 SDK | 애플리케이션 안에서 Claude Code의 도구 사용, 세션, 권한을 갖춘 에이전트 루프를 실행하기 위한 TypeScript·Python SDK입니다. | [Agent SDK 개요](https://code.claude.com/docs/en/agent-sdk/overview) |
| agent team | 에이전트 팀 | 리드 세션과 여러 팀원 세션이 공유 작업 목록과 메시지로 협업하는 Claude Code의 실험 기능입니다. | [Agent teams](https://code.claude.com/docs/en/agent-teams) |
| subagent | 서브에이전트 | 주 에이전트가 독립 하위 작업을 위임하고 결과를 받는 작업 단위입니다. | [Agents](https://code.claude.com/docs/en/agents) |
| Remote Control | 원격 제어 | 다른 기기에서 로컬 컴퓨터의 Claude Code 세션을 이어서 제어하는 연구 미리보기 기능입니다. | [Remote Control](https://code.claude.com/docs/en/remote-control) |
| Plan mode | 계획 모드 | 파일 변경 전에 계획을 세우고 검토하도록 제한하는 Claude Code 권한 모드입니다. | [Permission modes](https://code.claude.com/docs/en/permission-modes) |
| Model Context Protocol (MCP) | 모델 컨텍스트 프로토콜 | AI 애플리케이션이 외부 도구와 데이터 소스에 연결할 수 있도록 하는 개방형 프로토콜입니다. | [Claude Code MCP](https://code.claude.com/docs/en/mcp) |
| hook | 훅 | Claude Code 생명주기 이벤트에 연결해 결정적 검증 또는 자동화를 수행하는 핸들러입니다. | [Hooks](https://code.claude.com/docs/en/hooks) |
| skill | 스킬 | Claude가 필요할 때 불러 재사용하는 지침과 워크플로 묶음입니다. | [Skills](https://code.claude.com/docs/en/skills) |
| plugin | 플러그인 | skills, agents, hooks, MCP 설정 등을 묶어 배포·공유하는 확장 패키지입니다. | [Plugins](https://code.claude.com/docs/en/plugins) |
| prompt injection | 프롬프트 인젝션 | 웹 문서나 외부 도구 결과에 섞인 지시가 모델의 원래 작업 또는 보안 경계를 바꾸도록 유도하는 공격·위험입니다. | [Security](https://code.claude.com/docs/en/security) |
| worktree | 워크트리 | 하나의 Git 저장소에서 별도 작업 디렉터리와 브랜치를 함께 사용해 변경을 격리하는 Git 기능입니다. | [Agent teams와 worktrees](https://code.claude.com/docs/en/agent-teams) |
