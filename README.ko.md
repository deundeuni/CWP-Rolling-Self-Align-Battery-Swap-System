> **다국어 공개 안내:** 본 문서는 동일 내용의 한/영 이중 공개 문서입니다. v2.2 2026-09-13 (영문: [README_EN.md](README_EN.md))  
> **Original Authority Notice:** 본 기술 명세의 법적·공학적 판단 최상위 기준은 한글 원본(`README.ko.md`)에 귀속되며, 영문본은 보조 참조용으로만 기능한다. (PHILOSOPHY.ko.md is authoritative original)

# CWP 회전식 자율 정렬 배터리 교환 시스템 v2.2 - 중대형 및 소형 플랫폼 (범용 중량물·소형 모듈 페일세이프 기구적 정렬 플랫폼의 배터리 적용 실시예)

* **공개 일자:** 2026-09-13 (초안 2026-08-20, v2.0 2026-08-23, v2.1 2026-09-06, v2.2 2026-09-13)
* **작성자:** deundeuni (System Architect / Natural Person Inventor)
* **라이선스:** CERN-OHL-S v2 (하드웨어/CAD/도면) | CC BY-SA 4.0 (문서/설명)
* **공개 목적:** 방어적 공개 / 선행기술(Prior Art) 등록 - 독점 특허화 방지 및 권리 침해 위험 완화
* **검색 키워드:** CWP, CWP-Rolling-Self-Align, EV 배터리 교환, 자율 정렬, V홈 가이드, Passive Self-Align, Rolling Rail, Type A, Type B, Type C, Type S, Battery Swap, Height Adjustable Caster, Low Impact Docking, Prior Art, CWP-Entry, CWP-Battery-Swap, CWP-Clamping, 범용 중량물 정렬, Heavy Payload Alignment Platform, Off-Grid Self-Align, 노지 중량 모듈 정밀 정렬

---

## 0. 설계자 독자 아키텍처 및 선행기술 공개 선언 (Designer's Philosophical Declaration)

1. **설계 철학 및 기술 조합의 독자성 (Architectural Conception):**  
   본 시스템은 야외 노지 환경, 정전, 승객 갇힘 등 열악한 현장 여건에서도 고가의 전용 서보 설비 없이 기계식 수동 정렬(Passive Self-Align)을 통해 안전한 도킹 및 결합을 달성하고자 하는 **설계자(deundeuni)의 독자적 철학과 문제 의식**에서 출발하였다. 'V홈 가이드 + 높이조절 캐스터 + 슬라이딩 롤링 레일'의 3단 기계 메커니즘을 착안하고, 모듈형 체계(Type A/B/C 및 Type S) 및 파라미터 수치 범위를 결합·정립한 아키텍처 결정권은 설계자 자연인에게 있다.

2. **소프트웨어 유틸리티 활용에 관한 명시 (Software Utility Limitation):**  
   본 문서 작성 과정에서 활용된 소프트웨어 및 AI 도구는 설계자가 이미 정의한 기술 조합, 설계 방향, 수치 파라미터를 바탕으로 단순 포맷팅, 문맥 정제, 개념 시각화 출력을 실행한 **수동적 실행 유틸리티(Passive Execution Utility)**에 국한된다. 본 인프라의 모든 설계 의도, 구조적 결합권, 선행기술 공개 권한은 전적으로 설계자 자연인에게 귀속된다.

---

## 1. 설계 본질 및 적용 범위

### 1.1 메커니즘 본질 — 외형이 아닌 기계 구조가 본질
본 시스템은 시각적 외형이나 특정 탑재물에 고착되지 않고, 표준 기계 요소의 3단 결합 메커니즘을 기술적 본질로 한다.

* **이송 구조 (Transport):** 롤링 레일 위 슬라이딩 이송 방식으로 저마찰 직선 운동을 지원함.
* **정렬 형식 (Alignment Format):** V홈 가이드 25°~50° 범위 (바람직하게는 30°~45°)와 높이조절 캐스터 결합을 통한 기계적 수동 자율 정렬(Passive Self-Align) 모듈 구조.
* **모듈화 형식 (Modular Format):** 동일 레일 규격을 유지하며 환경 및 용도에 따라 프레임 모듈을 선택 교체하는 구조.

### 1.2 적용 범위 (Application Scope)
본 구조는 EV 배터리 교환에 한정되지 않으며, 노지 및 부평탄 지형에서 중량 모듈러 주택, 재난 대피소, 농기계 모듈, 물류 파렛트 등 500kg 이상 중량물 및 소형 모듈 페이로드의 물리적 치수 오차 흡수 및 정밀 기구적 결합에 범용으로 적용 가능하다. EV, ESS, 물류로봇(AGV/AMR), 드론, 선박, 항공우주, 건설·농업용 중장비 모듈 등 페이로드 착탈 및 정렬이 필요한 전 분야를 포괄한다.

---

## 2. Type A / B / C - 중대형 플랫폼 (Heavy Platform)

### 2.1 환경 적응형 타입 분류

* **Type A (평탄한 실내):** 고정식 기본 레일 구조 기반 정밀 정렬 지향 형식.
* **Type B (야외 노지 - 핵심):** V홈 자율 정렬 가이드 및 높이조절 캐스터 결합으로 지면 요철 및 세사 오차를 유연하게 흡수하는 노지 대응 형식.
* **Type C (중장비 현장):** 보강형 H빔 스틸 프레임 구조 기반 고하중 지지 형식.

### 2.2 기술 사양 (Heavy)

* **[권리범위 비한정 선언]** 본 문서의 모든 치수·각도·재질은 이해를 돕기 위한 일 실시예(One Embodiment)이며, 동일 기능(롤링 이송 + V홈 자율정렬)을 구현하는 범위 내에서의 수치 변경, 재질 변경 및 변형 응용은 본 선행기술의 범주에 포함된다.

* **주 프레임:** 20x20mm 내지 40x40mm급 표준 알루미늄 프로파일 또는 동등 강성의 H빔 (실시예: 20x20, 4040)
* **정렬 가이드:** V홈 25°~50° 범위 (바람직하게는 30°~45°) (실시예: 30°)
* **구동 방식:** 밀폐형 볼베어링 롤러 및 저마찰 베어링 구조
* **공차 흡수:** ±3mm~±10mm 범위의 플로팅 구속 (실시예: ±5mm)

---

## 3. Type S - 소형 플랫폼 (Small Platform)

중대형 수동 자율 정렬 원리를 소형 배터리 및 소형 모듈 규격에 맞춰 경량화한 모듈 형식이다.

* **이송 구조:** 20x20mm급 알루미늄 프로파일 레일 + 슬라이딩 캐리지 결합
* **정렬 형식:** 미니 V홈 25°~50° 범위 (실시예: 30°) + 20mm~50mm급 저상형 캐스터 (실시예: 25mm, ±5mm 자율 정렬 완화)
* **기구적 사양:** 중량 1.0kg~3.0kg 범위 (실시예: 1.8kg) / 길이 250mm~400mm 범위 (실시예: 320mm) / 70mm~120mm 저상형 (실시예: 95mm) / 무공구 걸쇠(Tool-less latch) 결합
* **상세 규격:** (실시예: 320 x 120 x 95 mm / 1.8 kg, 상기 권리범위 내 변형 가능)
* **전기 사양:** 12V~48V 범위 (실시예: 24V 5Ah) / XT30 내지 동등 규격 커넥터 / 동작 온도 -20°C ~ 60°C 범위
* **적용 대상:** 전동 스쿠터, 전동 공구, 소형 물류 로봇(AGV/AMR), 드론 landing skid, 소형 센서 모듈 등 전 분야

---

## 3.5 CWP 3대 하드웨어 연계 및 생존 아키텍처 (CWP 3-Hardware & System Integration)

본 기계적 셀프 얼라인 구조(Type B/S)는 단독 작동에 그치지 않고 CWP 3대 핵심 하드웨어 메커니즘 및 상위 생존 아키텍처와 유기적으로 결합되어 무중단 생존 지향형 교환 스테이션 및 정밀 도킹 인프라로 동작할 수 있다.

* **진입 유도 및 1차 정렬 (`CWP-Entry`):** 세차장 V레일 및 지면 가이드 홈 인프라 원용과 라인 레이저 가이드를 통해 진입 오차를 완화하고 정비 구역으로 유도함.
* **기구적 2차 정렬 (`CWP-Rolling-Self-Align-Battery-Swap-System` - 본 기술):** V-홈 및 캐스터 수동/자율 정렬 메커니즘(A/B/C/S 타입)과 연동하여 진입 후 치수 오차(예: ±5mm 이상)를 물리적으로 흡수하고 정밀 도킹 구역으로 유도함. (배터리 팩 및 500kg 이상 범용 중량 모듈 공통 적용)
* **차동 감속 저충격 도킹 (`CWP-Battery-Swap`):** N/(N+1) 차동 기어비(예: 60T/61T) 및 회전형 스테이지를 활용하여 도킹 상대속도를 극저속(예: 0.016rpm 수준)으로 감속시켜 완충 도킹을 지향함.
* **전자기 클램핑 및 안전 체결 (`CWP-Clamping-Battery-Swap-System`):** 범용 EPM 마그네틱 클램핑 모듈, 이중 핀 고정 및 3중 쿠션 구조와 결합하여 정밀 정렬 후 무전력 영구자석 고정 및 비상시 안전 해제를 지향함.
* **물리적 비상 차단·해제 (`0.1ms HW Intercept` / `LAST-LIGHT` 연계):** 화재, 정전 등 비상 상황 발생 시 Hardware Intercept 신호에 의해 체인, 공압, EPM 클램프가 릴리즈(Release)되어 무전력 기계식 이탈 및 탈출을 지원함.
* **연산적 제어 생존 (`chiplet-apu-multi-system-survival-architecture`):** 분산 관제(CCS) 및 다중 칩렛 제어 아키텍처와 결합하여 관제 칩렛 고장 시에도 정렬 및 교환 로직이 지속 동작하도록 구성함.

---

## 4. 한계, 보증 부인 및 면책 (Limitation, Disclaimer of Warranties & Liability)

본 문서는 방어적 공개를 위한 기술적 개념 개시이며, 어떠한 보증도 없이 있는 그대로(AS-IS) 제공된다.

1. **보증 부인:** 특정 목적 적합성, 상품성, 안전성, 제품화를 보증하지 않는다.
2. **책임 제한:** 본 문서의 사용, 구현, 응용으로 인한 직접·간접 손해, 사고, 손실에 대해 작성자(deundeuni)는 어떠한 법적 책임도 지지 않는다.
3. **제3자 권리 비보증:** 본 문서가 제3자의 특허, 상표, 저작권 등 권리를 침해하지 않음을 보증하지 않으며, 권리 조사는 구현자의 책임이다.
4. **법규·안전·인증 책임:** 각 국가의 법규, 전기·소방·안전 기준, 인증 획득 및 안전 검증 책임은 전적으로 구현자에게 있다.

---

## 5. 도면 및 인공지능 시각화 면책 (Figures & AI Visualization Disclaimer)

* **주의 (AI 시각화 면책 조항):** 본 명세서의 메커니즘 개념은 작성자(deundeuni)가 독자적으로 고안했습니다. 첨부된 도면 및 개념도는 이해를 돕기 위해 범용 생성형 AI 시각화 도구를 활용하여 생성된 예시일 뿐이며, 기존 상용 제품이나 타인의 등록 특허 도면을 복제한 것이 아닙니다.
* **도면 비고:** 본 도면에 포함될 수 있는 모든 치수, 각도, 수량은 예시이며 범위를 한정하지 않는다. V홈 자율 정렬, 롤링 레일, 캐스터 결합 기능 구조만이 본 공개의 핵심이다.

---

## 6. 라이선스 및 상업적 이용 안내 (Licensing)

```text
CERN Open Hardware Licence Version 2 - Strongly Reciprocal (CERN-OHL-S v2)
Copyright (c) 2026 deundeuni

This hardware design is licensed under CERN-OHL-S v2.
You may manufacture and distribute it, even commercially,
but if you distribute products based on it, you must also
make the modified design files available under the same license.

Full text: [https://ohwr.org/cern_ohl_s_v2.pdf](https://ohwr.org/cern_ohl_s_v2.pdf)

Documentation and figures: CC BY-SA 4.0
[https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)
```

* **상업적 이용 안내:** 상업적 제조/판매 모두 가능함. CWP 부분을 개선한 도면만 같은 라이선스로 공개하면 되며, 귀사의 다른 비밀 설계까지 공개할 필요는 없음.

---

## 7. 실리보호 (Practical Protection)

* **원안 우선 원칙:** 본 명세서의 법적·기술적 해석은 한국어 원본(`README.ko.md`)을 최우선 기준으로 적용하며, 영문본 및 기타 언어 번역본은 참고용으로만 기능한다.
* **범위 포괄성:** 본 문서에 기술된 레일 규격, V홈 각도, 공차 흡수 수치, 캐스터 방식 등은 광범위한 선행기술 선점을 위한 예시로서 상위개념으로 포괄 적용된다.
* **사업화 내용 분리:** 본 백서 원안에는 Pure Open Source 및 선행기술 개시 내용만을 포함하며, 독자적인 수익 모델 및 사업화 세부 실행안은 별도 기술 문서로 분리 관리한다.

---

## 8. 출처 및 기록 (Sources & Records)

* **소마모아 생태계 저장소 및 학술 식별자 (Ecosystem Repositories & DOIs)**
  * 상위 범용 생존 아키텍처 & APU 연산 제어기 (`chiplet-apu-multi-system-survival-architecture`) — GitHub: `deundeuni / chiplet-apu-multi-system-survival-architecture` | CERN Zenodo DOI: `10.5281/zenodo.22374987` (https://doi.org/10.5281/zenodo.22374987)
  * 재난 피난 유도 & 보조 인프라 (`LAST-LIGHT`) — GitHub: `deundeuni / LAST-LIGHT` | CERN Zenodo DOI: `10.5281/zenodo.22373189` (https://doi.org/10.5281/zenodo.22373189)
  * CWP 롤링 셀프얼라인 (`CWP-Rolling-Self-Align-Battery-Swap-System`) — CERN Zenodo DOI: `10.5281/zenodo.22373704` (https://doi.org/10.5281/zenodo.22373704)
  * CWP 배터리 교환 도킹 (`CWP-Battery-Swap`) — CERN Zenodo DOI: `10.5281/zenodo.22373538` (https://doi.org/10.5281/zenodo.22373538)
  * CWP 전자기 클램핑 (`CWP-Clamping-Battery-Swap-System`) — CERN Zenodo DOI: `10.5281/zenodo.22373722` (https://doi.org/10.5281/zenodo.22373722)
  * CWP 진입 유도 정렬 (`CWP-Entry`) — GitHub: `deundeuni / CWP-Entry`
  * 최상위 거점 관문 및 메인 저장소 (`soma-moa`) — GitHub: `deundeuni / soma-moa` | 관문 도메인: `somamoa.ai.kr`

* **법적 근거 및 선사용권 규정 (Legal Statutes & Precedents)**
  * 대한민국 특허법 제103조 — 선사용에 의한 통상실시권
  * 미국 특허법 35 U.S.C. §273 — Defense to Infringement Based on Prior Commercial Use
