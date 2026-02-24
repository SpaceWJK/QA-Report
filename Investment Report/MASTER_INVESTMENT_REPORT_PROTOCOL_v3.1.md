# MASTER INVESTMENT REPORT PROTOCOL v3.1

**최종 업데이트**: 2026-02-24
**변경 사항**: 섹션 구조 및 Smith 분석 배치 규칙 명확화

---

## 핵심 원칙 (CRITICAL)

### 1. 섹션 타이틀 규칙
```yaml
Executive Summary: 영어 (필수)
나머지 섹션 1~10: 한국어

예시:
  - Executive Summary
  - 1. 최근 실적 분석
  - 2. 가이던스 및 전망
  - 10. 투자 전략
```

### 2. Smith 분석 배치 규칙
```yaml
금지:
  - 각 섹션마다 "Smith 분석" 박스 반복
  - Section 1~9에 Smith 평가/판단 삽입

허용:
  - Section 10 "투자 전략"에만 Smith 종합 평가
  - 팩트 서술 중 자연스러운 해석 (단, "Smith 분석:" 박스 형태 금지)

목적:
  - Section 1~9 = 팩트 기반 정보 전달
  - Section 10 = Smith의 종합 판단 및 실행 전략
```

### 3. 콘텐츠 품질 우선
```yaml
중요도:
  정보의 질 > 가시성 > 구조 > 줄 수

각 섹션 목표:
  - 핵심 팩트를 명확히 전달
  - 최신 데이터 우선
  - 시각적 가독성 (카드, 색상, 아이콘)
  - 불필요한 장황함 제거
```

---

## 표준 섹션 구조

### Executive Summary (영어)
- 투자 의견 (BUY/HOLD/SELL)
- 목표 주가
- 리스크 수준
- 투자 기간
- 핵심 투자 논리 (3~5개)
- 주요 리스크 (3~5개)

### 1. 최근 실적 분석
- 최근 분기/연간 실적
- 매출, 순이익, EPS, 마진
- 전년 대비 성장률
- 세그먼트별 매출
- **Smith 분석 금지**

### 2. 가이던스 및 전망
- 경영진 가이던스
- 애널리스트 컨센서스
- 중장기 성장 동인
- **Smith 분석 금지**

### 3. 밸류에이션
- P/E, P/S, PEG, EV/Sales
- 동종업계 비교
- 애널리스트 목표가 분포
- **Smith 분석 금지**

### 4. 시장 지위 및 경쟁 우위
- 시장 점유율
- 경쟁사 비교
- 기술적/구조적 경쟁력
- **Smith 분석 금지**

### 5. 재무 안정성
- 현금, 부채, 유동성
- FCF, ROE, ROA
- 신용등급
- **Smith 분석 금지**

### 6. 성장 전략
- 신규 사업/제품
- 지역 확장
- M&A 계획
- **Smith 분석 금지**

### 7. 리스크 요인
- 경쟁 리스크
- 규제/지정학
- 재무 리스크
- **Smith 분석 금지**

### 8. 인사이더 거래
- 최근 내부자 매수/매도
- 기관 투자자 지분 변화
- **Smith 분석 금지**

### 9. 최근 뉴스 및 이벤트
- 어닝콜 하이라이트
- 중요 발표
- 산업 이벤트
- **Smith 분석 금지**

### 10. 투자 전략 ⭐
**이 섹션에만 Smith 종합 평가 집중**
- Smith 최종 투자 의견
- 목표가 시나리오 (Bull/Base/Bear)
- 매수/매도 가격대
- 분할 매수 전략
- 손절/익절 규칙
- 모니터링 지표

---

## 디자인 일관성 (절대 규칙)

### 고정 요소
```yaml
CDN:
  - Tailwind CSS: v2.2.19
  - FontAwesome: v6.4.0
  - Google Fonts: Inter

CSS 클래스 (변경 금지):
  - .gradient-bg
  - .card-shadow
  - .metric-card
  - .section-header
  - .status-positive / negative / neutral

브랜드 색상만 변경:
  - .{ticker}-primary (예: .crwd-primary)
  - .{ticker}-bg
```

---

## 금지 사항

❌ Section 1~9에 "Smith 분석:" 박스 삽입
❌ Executive Summary를 한국어로 작성
❌ 매 섹션마다 평가/판단 반복
❌ 줄 수 늘리기 위한 장황한 서술
❌ Tailwind 버전 변경
❌ Inter 폰트 변경

---

## QA 체크리스트

### 구조 검증
- [ ] Executive Summary 영어 확인
- [ ] Section 1~10 한국어 확인
- [ ] 총 10개 섹션 존재
- [ ] Section 1~9에 "Smith" 키워드 없음
- [ ] Section 10에만 Smith 종합 평가 존재

### 디자인 검증
- [ ] Tailwind v2.2.19
- [ ] FontAwesome v6.4.0
- [ ] Inter 폰트
- [ ] .gradient-bg, .card-shadow 존재
- [ ] 브랜드 색상 클래스 적용

### 콘텐츠 품질
- [ ] 각 섹션 최신 데이터 포함
- [ ] 팩트 기반 서술
- [ ] 시각적 가시성 (카드, 색상)
- [ ] 불필요한 장황함 없음

