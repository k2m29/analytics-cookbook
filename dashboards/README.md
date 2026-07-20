# 📊 Dashboards & Data Governance 산출물

> ⚠️ 아래 이미지는 재직 중 직접 설계·운영한 실물 산출물을 **가명 데이터로 재현한 샘플**입니다.
> 게임명·테이블명·코드값·수치는 모두 가공된 것이며, 실데이터가 아닙니다. 구조·산식·운영 방식은 실물과 동일합니다.

## 1. GMV Breakdown 대시보드 (Tableau)

프로모션 상품(AID) 단위로 거래액을 리워드 유형별로 분해하는 일간 모니터링 뷰.

- **상단**: 일자별 거래액을 순결제·쿠폰·포인트·멤버십으로 스택, 매출·공헌이익 추정 라인 오버레이 → 프로모션이 "매출을 만든 건지, 마진을 태운 건지"를 하루 단위로 판별
- **하단**: CCP(쿠폰·캐시·포인트) 동반 발생 거래액을 리워드별 비중으로 분해하고, 포인트백 진행일에는 참여 발생 거래액(보라)을 병렬 표시 → 리워드 투입 대비 동반 매출 확인

![GMV Breakdown](images/gmv_breakdown_sample.png)

## 2. Game Tracking — 주차별 게임 포지셔닝 (Tableau Pages)

X=신규 다운로더, Y=거래액(로그-로그) 산점도에 Tableau Pages 히스토리 트레일을 적용해 **주차별로 게임이 어디서 어디로 이동했는지** 추적. 크기=평균 유료구매자, 빨간 테두리=최근 3개월 신작. 신작의 초기 궤적과 기존작의 이탈 신호를 한 화면에서 감지.

![Game Focus](images/game_focus_sample.png)

## 3. 이벤트 퍼널 대시보드 (Tableau)

쿠폰 이벤트를 **발급유저 → 사용자 → 사용율 → 소진율 → 발생거래액 → CCP% → ROAS% → 결제/쿠폰단가** 퍼널로 표준화한 결과표. 헤더에 산식 정의를 문서화해 이해관계자 간 지표 해석 차이를 제거. 릴레이형 쿠폰(1~5단계)의 단계별 잔존율로 설계 효율을 검증.

![Coupon Funnel](images/coupon_funnel_sample.png)

## 4. 시간감쇠 기반 신작 랭킹 — 프로덕션 실화면

2019년에 설계한 신작 랭킹 알고리즘(신선도 부스트 + 다중 지표 정규화 가중합)이 적용된 **'최신출시' 탭의 현재 실서비스 화면**입니다. 기존 인기·매출 랭킹을 신작이 뚫지 못하는 문제를 해결하기 위해 설계했고, 개발 이관 후 현재까지 프로덕션에서 운영 중입니다. 공개된 앱 화면이므로 마스킹 없이 게시합니다.

<img src="images/ranking_newrelease_live.png" alt="New Release Ranking — Live" width="360">

## 5. SQL Dictionary (SharePoint 위키)

분석 쿼리 표준화를 위해 직접 구축·운영한 사내 위키. "같은 지표인데 사람마다 숫자가 다른" 문제를 기준정의 문서화로 해결.

### 홈 — Dictionary & News + SQL Sample 목록
기준정의/집계/예제 구분, 업무영역 태그, 재사용 가능한 [CTE] 모듈, 관련 문서 연결.

![SQL Dictionary Home](images/sql_dictionary_home_sample.png)

### 상세 페이지 — 전사 표준 거래액 정의
산식 + 제외조건 + 검증용 대시보드 링크 + 주석 달린 base 쿼리. "정의용 base이므로 집계는 목적에 맞게 별도 작성" 등 사용 가이드 포함.

![SQL Dictionary Detail](images/sql_dictionary_detail_sample.png)

### ERD — 포인트 도메인
테이블 간 조인키를 명시하고, 포인트 *지급 예정액 / 지급액 / 사용액*이 각각 어느 테이블·컬럼에서 나오는지 주석으로 구분.

![SQL Dictionary ERD](images/sql_dictionary_erd_sample.png)

### Table Dictionary — 컬럼 사전 & 코드 조견표
주요 테이블의 컬럼 정의(타입·설명·샘플값)와 코드성 컬럼의 CODE_NM 시트 상호참조. 결제수단·리워드·이벤트 유형 코드를 한 곳에서 조회.

![Table Dictionary](images/table_dictionary_main_sample.png)

![Code Sheet](images/table_dictionary_codenm_sample.png)
