---
marp: true
theme: gaia
class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
style: |
  @import url('https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/static/pretendard.css');

  :root {
    --color-primary: #2563eb;
    --color-secondary: #7c3aed;
    --color-before: #dc2626;
    --color-after: #16a34a;
    --color-bg-before: #fef2f2;
    --color-bg-after: #f0fdf4;
    --color-border-before: #fca5a5;
    --color-border-after: #86efac;
    --color-section-bg: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  }

  section {
    font-family: 'Pretendard', 'Apple SD Gothic Neo', 'Malgun Gothic', sans-serif;
    font-size: 28px;
    padding: 40px 60px;
  }

  section.lead h1 {
    font-size: 2.2em;
    color: #1e293b;
  }

  section.lead h2 {
    font-size: 1.4em;
    color: #475569;
    font-weight: 400;
  }

  h1 {
    color: #1e293b;
    font-weight: 700;
    border-bottom: 3px solid var(--color-primary);
    padding-bottom: 10px;
  }

  h2 {
    color: #334155;
    font-weight: 600;
  }

  /* Before/After 레이아웃 */
  .compare {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    margin-top: 20px;
  }

  .before {
    background: var(--color-bg-before);
    border: 2px solid var(--color-border-before);
    border-radius: 12px;
    padding: 20px 24px;
  }

  .before h3 {
    color: var(--color-before);
    margin: 0 0 12px 0;
    font-size: 1.1em;
  }

  .after {
    background: var(--color-bg-after);
    border: 2px solid var(--color-border-after);
    border-radius: 12px;
    padding: 20px 24px;
  }

  .after h3 {
    color: var(--color-after);
    margin: 0 0 12px 0;
    font-size: 1.1em;
  }

  .before ul, .after ul {
    margin: 0;
    padding-left: 20px;
    font-size: 0.85em;
    line-height: 1.8;
  }

  /* 섹션 구분 슬라이드 */
  section.section-divider {
    background-color: #667eea !important;
    background-image: linear-gradient(135deg, #667eea 0%, #764ba2 100%) !important;
    color: white;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  section.section-divider h1 {
    color: white !important;
    border-bottom: none;
    font-size: 2.4em;
  }

  section.section-divider p {
    font-size: 1.2em;
    opacity: 0.9;
    color: white !important;
  }

  /* 하이라이트 박스 */
  .highlight {
    background: #eff6ff;
    border-left: 4px solid var(--color-primary);
    padding: 16px 20px;
    border-radius: 0 8px 8px 0;
    margin: 16px 0;
    font-size: 0.95em;
  }

  /* 비교 테이블 */
  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.82em;
    margin-top: 12px;
  }

  th {
    background: #2563eb;
    color: white;
    padding: 10px 14px;
    text-align: left;
  }

  td {
    padding: 10px 14px;
    border-bottom: 1px solid #e2e8f0;
  }

  tr:nth-child(even) {
    background: #f8fafc;
  }

  /* 시간 절감 배지 */
  .time-save {
    display: inline-block;
    background: #16a34a;
    color: white;
    padding: 4px 14px;
    border-radius: 20px;
    font-size: 0.8em;
    font-weight: 600;
    margin-top: 8px;
  }

  /* CTA 스타일 */
  .cta-steps {
    counter-reset: step;
  }

  .cta-step {
    background: #f8fafc;
    border-radius: 12px;
    padding: 16px 20px;
    margin: 10px 0;
    display: flex;
    align-items: center;
    gap: 16px;
    font-size: 0.9em;
  }

  .cta-step .num {
    background: var(--color-primary);
    color: white;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 700;
    flex-shrink: 0;
  }

  .emoji-big {
    font-size: 3em;
    margin-bottom: 16px;
  }

  footer {
    font-size: 0.6em;
    color: #94a3b8;
  }

---

<!-- _class: lead -->
<!-- _paginate: false -->

# AI, 이제 대화만 하는 게 아닙니다

## 채팅에서 실행으로 — 에이전트 AI가 바꾸는 업무의 미래

<br>

2026년 2월 | 사내 세미나

---

# 🤖 지금 우리가 아는 AI

<br>

### 질문하면 답해주는 **"전화 상담원"**

- 💬 "이 데이터 어떻게 분석하면 될까?" → 방법을 **알려줌**
- 💬 "보고서 초안 써줘" → 텍스트를 **생성**해줌
- 💬 "이 표현 영어로 번역해줘" → 번역을 **보여줌**

<div class="highlight">

핵심: AI가 **말해주면**, 실행은 **내가 직접** 한다
복사 → 붙여넣기 → 서식 정리 → 저장 → 공유... 🔄

</div>

---

# 😤 이런 적 없으셨나요?

<br>

| 상황 | 채팅 AI의 한계 |
|------|---------------|
| 📁 "이 엑셀 파일 정리해줘" | 파일을 직접 열 수 없음 |
| 📅 "내일 회의 잡아줘" | 캘린더에 접근할 수 없음 |
| 📧 "거래처에 메일 보내줘" | 이메일을 보낼 수 없음 |
| 🗄️ "지난달 매출 뽑아줘" | 데이터베이스 조회 불가 |

<br>

> 결국 **"방법은 알겠는데, 실행은 내가 해야 하잖아..."** 😅

---

# 💡 에이전트 AI = 직접 일하는 AI

<br>

<div class="compare">
<div class="before">
<h3>❌ 채팅 AI (지금)</h3>

- "이렇게 하면 됩니다"
- 텍스트로만 답변
- 한 번에 한 가지 질문
- 도구 사용 불가

</div>
<div class="after">
<h3>✅ 에이전트 AI (진화)</h3>

- "제가 해드리겠습니다"
- 파일, 앱, 시스템 직접 조작
- 여러 단계를 스스로 판단·실행
- 도구를 조합해서 업무 완수

</div>
</div>

<div class="highlight">

🔑 핵심 차이: **"알려줄게"** → **"내가 해줄게"**
AI가 도구를 사용하고, 스스로 판단하여 업무를 끝까지 처리

</div>

---

<!-- _class: section-divider -->

<div class="emoji-big">📄</div>

# 문서 & 데이터 처리

업무 시간의 40%를 차지하는 반복 작업

---

# 📊 경영 보고 자료 취합

<div class="compare">
<div class="before">
<h3>❌ Before</h3>

- 부서별 현황 엑셀 여러 개 수집
- 수동으로 데이터 취합·교차 검증
- 경영층 보고 양식에 맞춰 재정리
- 파워포인트로 도표·차트 제작
- ⏱️ **약 3시간 소요**

</div>
<div class="after">
<h3>✅ After</h3>

- "이번 달 현황 보고서 정리해줘"
- AI가 파일 자동 수집·비교·취합
- 보고 양식에 맞춘 도표 자동 생성
- 이상치·변동 포인트 자동 하이라이트
- ⏱️ **약 10분 소요**

</div>
</div>

<span class="time-save">⏱️ 약 95% 시간 절감</span>

---

# 📈 인력·조직 현황 분석

<div class="compare">
<div class="before">
<h3>❌ Before</h3>

- 인사 시스템에서 데이터 추출
- 피벗테이블로 부서별·직급별 정리
- VLOOKUP으로 여러 시트 연결
- 분석 결과 해석·요약은 별도 작업
- ⏱️ **반나절~하루**

</div>
<div class="after">
<h3>✅ After</h3>

- "부서별 인력 현황 분석해줘"
- 자연어로 질문하면 자동 분석
- 적합한 시각화 차트 자동 생성
- 증감 추이와 시사점까지 요약
- ⏱️ **5~15분**

</div>
</div>

<span class="time-save">⏱️ 약 90% 시간 절감</span>

---

<!-- _class: section-divider -->

<div class="emoji-big">⚙️</div>

# 워크플로우 자동화

사람의 판단이 필요한 곳에만 사람이 개입

---

# 🧾 회의 준비 & 의사록 정리

<div class="compare">
<div class="before">
<h3>❌ Before (다단계 수동)</h3>

- ① 지난 회의록에서 후속과제 확인
- ② 각 부서 담당자에게 진행상황 요청
- ③ 취합 후 안건별 자료 재구성
- ④ 회의 후 의사록 수기 정리
- ⑤ 결정사항·후속과제 배포
- ⏱️ **회의당 2~3시간**

</div>
<div class="after">
<h3>✅ After (AI 자동화)</h3>

- ① 이전 회의록 기반 후속과제 자동 추적
- ② 진행상황 자동 취합·요약
- ③ 안건별 보고자료 초안 생성
- ④ 회의 녹취 → 의사록 자동 작성
- ⑤ 결정사항·담당자별 할당 자동 배포
- ⏱️ **회의당 15~20분**

</div>
</div>

<span class="time-save">⏱️ 약 85% 시간 절감</span>

---

# 📢 임원 보좌 & 일정 관리

<div class="compare">
<div class="before">
<h3>❌ Before</h3>

- 매일 아침 일정·안건 수동 확인
- 관련 부서 자료 개별 요청·취합
- 브리핑 자료 수동 작성
- 출장·미팅 후 후속조치 수기 관리
- ⏱️ **매일 1~2시간**

</div>
<div class="after">
<h3>✅ After</h3>

- AI가 일정 변동·신규 안건 자동 감지
- 관련 자료 자동 수집·요약
- 브리핑 메모 초안 자동 생성
- 후속과제 자동 트래킹·리마인드
- ⏱️ **확인·수정만 10분**

</div>
</div>

<span class="time-save">⏱️ 주당 약 8시간 절감</span>

---

<!-- _class: section-divider -->

<div class="emoji-big">🚀</div>

# 일상 업무 생산성

조사 → 비교 → 정리 → 보고를 한번에

---

# 🔍 경쟁차 벤치마킹 자료 정리

<div class="compare">
<div class="before">
<h3>❌ Before</h3>

- 경쟁차 리뷰·스펙 자료 수동 검색
- 제원·가격·옵션 항목별 수동 정리
- 비교표 엑셀로 직접 작성
- 분석 결과 보고서로 재구성
- ⏱️ **2~3일 소요**

</div>
<div class="after">
<h3>✅ After</h3>

- "경쟁 모델 3종 비교 분석해줘"
- AI가 공개 자료 자동 수집·정리
- 항목별 비교표 + 강약점 자동 생성
- 위원회·보고용 초안까지 작성
- ⏱️ **약 30분 소요**

</div>
</div>

<span class="time-save">⏱️ 약 95% 시간 절감</span>

---

# 📋 한눈에 비교: 채팅 AI vs 에이전트 AI

<br>

| 구분 | 💬 채팅 AI | 🤖 에이전트 AI |
|------|-----------|--------------|
| **비유** | 전화 상담원 | 신입 인턴 |
| **역할** | 질문에 답변 | 업무를 직접 수행 |
| **도구 사용** | 텍스트만 생성 | 파일·앱·시스템 조작 |
| **작업 범위** | 1회성 응답 | 다단계 업무 처리 |
| **결과물** | 텍스트 답변 | 완성된 산출물 |

<div class="highlight">

💡 에이전트 AI는 채팅 AI의 **대체가 아닌 진화**입니다.
실제로 비개발 직군 임원이 30개 시트 엑셀 재무모델을 **프롬프트 2~3개로** 자동 분석 시스템으로 전환한 사례도!

</div>

---

<!-- _class: section-divider -->

<div class="emoji-big">⏰</div>

# 이 변화, 얼마나 된 걸까?

"아직 아무도 준비 못 했습니다"

---

# 📅 불과 3개월 전에 시작된 변화

<br>

| 시점 | 사건 | 의미 |
|------|------|------|
| **2025.11.24** | Claude Opus 4.5 출시 | 에이전트 AI 성능이 실무 수준 돌파 |
| **2026.01.12** | Claude Cowork 공개 | 비개발자도 에이전트 AI 사용 가능 |
| **2026.01~02** | 뉴욕 증시 SaaS 폭락 | Salesforce -14%, Adobe 5년 저점 |
| **지금** | 대부분의 직장인 | 아직 채팅 AI만 사용 중 |

<div class="highlight">

🔑 **3개월 만에** 기술 → 제품 → 시장 충격까지 연쇄 발생
지금 시작하면 늦은 게 아니라, **오히려 빠른 편입니다**

</div>

---

# 📉 월가가 먼저 반응했다

<br>

### "AI가 기존 소프트웨어를 대체한다" — SaaSpocalypse

- 📊 나스닥 100: 2주 만에 **시가총액 1조 달러 증발**
- 📉 Salesforce(CRM): 일주일 만에 **-14%**, 2023년 수준 복귀
- 📉 Adobe: **5년 만의 최저점** (2019년 수준)
- 📉 HubSpot -39%, Figma -40%, Atlassian -35%

<div class="highlight">

💡 주가 폭락의 이유: AI 에이전트가 **사람이 소프트웨어로 하던 일**을 직접 처리
→ 기존 SaaS 도구의 존재 이유 자체에 의문이 생긴 것

</div>

---

# ⚠️ 현실적 고려사항

<br>

### 🛡️ 기대만큼 중요한 주의점

- 👁️ **사람의 감독은 필수**
  AI가 처리한 결과는 반드시 사람이 검토·승인

- ⚖️ **100% 완벽하지 않음**
  특히 숫자, 날짜, 고유명사는 꼭 확인 필요

- 🔒 **보안과 권한 관리**
  민감한 데이터 접근 범위를 명확히 설정

- 📊 **AI 활용 격차가 벌어지고 있음**
  적극 활용하는 팀과 기본 채팅만 쓰는 팀의 생산성 차이가 급격히 확대 중

---

# 🎯 내일부터 시작할 수 있는 것

<br>

<div class="cta-step">
<div class="num">1</div>
<div><strong>관찰하기</strong> — 이번 주 내 업무 중 "이거 반복이다" 싶은 작업 3개 적기</div>
</div>

<div class="cta-step">
<div class="num">2</div>
<div><strong>실험하기</strong> — 그중 가장 간단한 1개를 AI 도구로 시도해보기</div>
</div>

<div class="cta-step">
<div class="num">3</div>
<div><strong>공유하기</strong> — 결과를 팀에 공유하고, 함께 확장할 업무 찾기</div>
</div>

<br>

> *"지금 두 가지 유형의 AI 사용자가 생기고 있습니다.
> 도구로 활용하는 사람과, 채팅에 머무는 사람.
> 그 격차는 이미 벌어지고 있고, 중요한 건 시작하려는 의지입니다."*

<!-- _footer: 감사합니다. 질문이 있으시면 편하게 말씀해주세요! 🙏 -->
