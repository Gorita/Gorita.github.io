---
title: "Pattern Scout: AI 에이전트 디자인 패턴 카탈로그"
date: 2026-01-22 10:00:00 +0900
categories: [Project, AI]
tags: [Pattern Scout, AI Agents, Design Patterns, Agentic Patterns]
---

AI 에이전트를 개발하다 보면 어떤 디자인 패턴을 적용해야 할지 막연할 때가 있습니다. ReAct, Chain-of-Thought, Tool Use 같은 용어들은 들어봤지만, 실제 문제 상황에 어떤 패턴이 적합한지 찾기는 쉽지 않습니다.

Pattern Scout는 이런 문제를 해결하기 위해 만든 웹 애플리케이션입니다.

## 무엇을 담고 있나요

[awesome-agentic-patterns](https://github.com/nibzard/awesome-agentic-patterns)의 117개 패턴을 정리했습니다. 각 패턴은 다음 정보를 포함합니다:

- 문제 정의와 해결 방법
- 다이어그램
- 코드 예제
- 장단점

패턴들은 8개 카테고리로 나뉩니다:

- **Orchestration & Control**: 태스크 분해, 에이전트 관리 (31개)
- **Context & Memory**: 컨텍스트 관리, 메모리 최적화 (13개)
- **Feedback Loops**: 피드백 기반 개선 (13개)
- **Learning & Adaptation**: 자가 학습, 적응 (5개)
- **Reliability & Eval**: 안정성, 평가 (13개)
- **Security & Safety**: 보안, 안전성 (3개)
- **Tool Use & Environment**: 도구 사용, 환경 통합 (26개)
- **UX & Collaboration**: 사용자 경험, 협업 (13개)

## 주요 기능

**검색**: 패턴 제목, 설명, 태그로 실시간 검색할 수 있습니다.

**이중 언어 지원**: 모든 패턴을 한국어와 영어로 제공합니다. 원문이 필요한 경우 언어를 전환하면 됩니다.

**반응형 디자인**: 모바일과 데스크톱 모두에서 사용할 수 있습니다.

## 기술 스택

- Astro: 정적 사이트 생성
- Tailwind CSS: 스타일링
- GitHub Pages: 호스팅

별도의 백엔드나 데이터베이스 없이 순수하게 정적 사이트로 구성되어 있습니다.

## 사용해보기

[https://gorita.github.io/pattern-scout](https://gorita.github.io/pattern-scout)

소스 코드는 [GitHub](https://github.com/Gorita/pattern-scout)에 공개되어 있습니다. 패턴 추가나 번역 개선에 대한 기여도 환영합니다.

---

AI 에이전트를 만들면서 "이런 상황에 어떤 패턴을 쓰면 좋을까?" 고민했던 분들께 도움이 되었으면 합니다.
