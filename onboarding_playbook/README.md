# 🌐 Partner Onboarding Knowledge Hub — App Store Operations

해외 파트너사가 화이트라벨 앱스토어를 **스스로 운영할 수 있도록**, 흩어져 있던 운영 노하우를 하나의 영어 기반 Knowledge Hub와 마케팅 플레이북으로 체계화한 프로젝트입니다.

단순한 문서 정리가 아니라, 신규 담당자가 별도 교육 없이도 자신의 역할에 맞는 정보를 찾아 업무를 수행할 수 있도록 **정보 구조(Information Architecture)와 온보딩 경험(User Journey) 자체를 설계**했습니다. 기존 문서 체계의 문제(지식 분산·반복 문의·특정 담당자 의존)를 발견하고 개선을 주도했으며, SharePoint의 정보 구조를 처음부터 직접 설계·단독 문서화했습니다.

> 🔒 **기밀 유지 안내** — 본 저장소의 모든 화면은 파트너사명, 내부 URL, 보안 정보, 예산, 할인율, 사용자 수 등 민감한 정보를 제거하거나 마스킹한 **재현 샘플**입니다. 공개 목적은 운영 데이터가 아니라 **정보 구조와 문서 설계 방식**을 소개하는 것입니다. 원문이 영어인 페이지는 영어를 유지했습니다.

---

## 1. 프로젝트 배경

해외 파트너사는 우리 플랫폼 기반으로 자체 앱스토어를 운영해야 했지만, 운영에 필요한 지식은 한국 운영자의 경험, 이메일 답변, 여러 내부 문서, 한국어 Wiki에 분산되어 있었습니다. 파트너사에는 Marketing, Operation, UXD, CS 등 다양한 직군이 있어 "문서를 한곳에 모아두는" 방식으로는 필요한 정보를 찾기 어려웠고, 그 결과 —

- 신규 담당자 교육에 많은 시간이 소요되고
- 동일한 질문이 반복되었으며
- 운영 경험이 특정 담당자에게 의존하는 문제가 발생했습니다.

**목표**: 운영 경험을 개인이 아닌 시스템에 축적하여, 신규 담당자가 영어 문서만으로 필요한 업무를 스스로 찾아 수행하는 **Self-service Onboarding 환경** 구축.

---

## 2. 구축한 것

### A. SharePoint Knowledge Hub (35+ 페이지 · 8개 카테고리)

**① 온보딩 중심 정보 구조** — 파일 목록 대신, 사용자가 실제 업무를 배우는 순서대로 이동하도록 설계:
*서비스 이해 → 환경 설정 → 운영 전략 → 관리자 시스템 → 데이터 활용 → FAQ*

**② 역할 기반(User Role) 정보 탐색** — 모든 문서에 Marketing / Operation / UXD / CS / All 태그를 부여해, 자신의 역할에 필요한 문서만 필터링해 읽도록 구성.

**③ 카테고리 설계(Taxonomy)** — Q&A, Marketing Operation, Admin Registration, Design Asset, Data, Customer Service, JIRA, Collaboration Tools & Environment의 8개 분류 + 부모-자식 구조(예: Promotion → Curation → Tile Design Guideline → Shortcut Card).

**④ 문서 템플릿 표준화** — 모든 운영 문서를 *정의 → 언제 사용하는가 → 업무 범위 → 업무 절차 → 관련 문서* 구조로 통일해, 어떤 문서를 열어도 같은 위치에서 같은 종류의 정보를 찾을 수 있게 함.

**⑤ Living Documentation** — 운영 중 반복되는 질문을 지속적으로 FAQ에 반영하고 Promotions Guide를 v1 → v2로 발전시키는 등, **1년 6개월 이상 운영하며 지식이 다시 문서로 돌아오는 선순환**을 유지.

#### Table of Contents — 온보딩 여정 + 역할 태그 목차

Getting Started가 학습 순서를 서사로 안내하고(여정), 아래 목차 표가 같은 페이지들을 카테고리·역할 태그로 재분류합니다(참조). 하나의 콘텐츠를 두 가지 경로로 찾게 하는 2중 내비게이션 구조.

![Table of Contents](images/help_toc_sample.png)

#### Marketing Overview — 파트너가 처음 읽는 문서

스토어 운영의 전체 그림(운영·외부 마케팅·CS·계약)과 Contents Provider → Store(HQ) → User 에코시스템, 본사/롤아웃 파트너(ROP)의 역할 분담을 다이어그램으로 정리.

![Marketing Overview](images/help_overview_sample.png)

#### Q&A — 반복 문의의 셀프서비스 전환

실제로 들어온 질문을 영/한 병기로 축적. 스크린샷과 함께 "어디서 막혔는지" 기준으로 작성해 문의 없이 스스로 해결하도록 유도. Living Documentation의 핵심 채널.

![Q&A](images/help_qna_sample.png)

### B. Marketing Playbook (34 Slides)

한국에서 축적된 프로모션 운영 경험을 해외 파트너가 그대로 활용할 수 있도록 제작한 플레이북. 기능 설명이 아니라 **실제 운영 전략과 의사결정 기준**을 전달하는 것이 목적입니다.

- **운영 프레임워크** — 게임 라이프사이클 × 고객 라이프사이클 × 앱스토어 런칭 단계, 세 관점에서 "언제 어떤 프로모션을 운영해야 하는지" 정리
- **프로모션 공통 프레임워크** — 모든 프로모션을 *Audience × Reward × Distribution* 3축으로 정의하고, Total Purchase / Actual Purchase / CCP 등 핵심 지표 정의를 표준화 → 파트너와 플랫폼 운영자가 같은 언어로 소통
- **프로모션 템플릿 표준화** — 12가지 프로모션을 *목적 → 사용자 Flow → 설정 방법 → KPI → 유의사항 → 실제 사례* 동일 형식으로 정리
- **운영 전략 제안** — 런칭 초기에는 단순한 프로모션부터, 대형 게임과의 협업 우선, 국가 특성에 맞는 현지화

#### Strategy & Promotion Samples — 플레이북의 웹 버전

플레이북 핵심 내용을 Knowledge Hub 페이지로도 제공. "Tip: In the launch stage" 등 실전 조언 섹션과 목표(획득/리텐션/개발사 지원)별 Marketing Portfolio 표.

![Strategy & Promotion Samples](images/help_promotion_sample.png)

---

## 3. 프로젝트 결과

- 해외 파트너의 Marketing, Operation, UXD, CS 담당자가 **하나의 영어 Knowledge Hub**를 기반으로 업무를 수행하는 환경 구축
- 반복 문의를 FAQ·운영 가이드에 반영해 **Self-service 기반 운영 문화** 형성
- 약 1년 6개월간 지속 개선하며 파트너 운영의 **Single Source of Truth** 역할 수행
- 담당 이관 후에도 후속 조직이 승계 운영 — 운영 노하우를 개인의 경험이 아닌 **조직의 자산**으로 전환

## 4. 이 프로젝트가 보여주는 역량

| 역량 | 내용 |
|---|---|
| Information Architecture | 사용자 역할과 온보딩 여정을 중심으로 정보 구조 설계 |
| Product Thinking | 조직 구조가 아닌 사용자의 업무 흐름에 맞춘 정보 경험 설계 |
| Knowledge Management | 반복 지원 업무를 재사용 가능한 문서로 전환하고 지속 관리 |
| Standardization | 문서·프로모션·KPI 정의를 표준화해 일관된 운영 체계 구축 |
| Cross-functional Communication | Marketing/Operation/UXD/CS가 동일한 기준으로 협업하는 공통 언어 구축 |
