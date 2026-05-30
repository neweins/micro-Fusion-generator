# 🚀 Micro-Fusion-generator (극소형 핵융합로 설계 연구)

고온 초전도체(2G HTS REBCO) 자석 공학 및 전자공학적 제어 기술을 기반으로 한 극소형 핵융합로(토카막) 설계 개인 연구 프로젝트입니다.

---

## 📚 1. 필수 전공 서적 (Textbooks)

전기/전자 엔지니어 관점에서 초전도 자석을 '시스템 및 회로'로 다루고 플라즈마의 거동을 이해하기 위한 바이블 서적입니다.

*   **High-Field Superconducting Magnets (Iwasa 저)**
    *   *설명:* MIT 이와사 교수의 초전도 자석 설계 교과서. 자석 내부의 기계적 스트레스, 저온 공학, 퀜치(Quench) 현상 및 보호 회로 설계 수록.
    *   *링크:* [SpringerLink 공식 페이지](https://springer.com)
*   **Case Studies in Superconducting Magnets (Iwasa 저)**
    *   *설명:* 위 교과서의 실무 버전. 구체적인 계산 예시와 설계 케이스가 담겨 있어 수치 계산 및 모델링 가이드로 적합.
    *   *링크:* [SpringerLink 공식 페이지](https://springer.com) / [Scribd 연구용 문서 목차](https://scribd.com)
*   **Plasma Physics and Controlled Fusion (Francis F. Chen 저)**
    *   *설명:* 플라즈마 물리학의 표준 교과서. 맥스웰 방정식을 기반으로 자기장 내 플라즈마 거동(MHD 이론)을 직관적으로 이해 가능.
    *   *링크:* [SpringerLink 공식 페이지](https://springer.com)

---

## 🔬 2. 핵심 벤치마킹 논문 (Research Papers)

MIT와 CFS(Commonwealth Fusion Systems)의 오픈소스 기반 극소형 고온 초전도 토카막(SPARC) 프로젝트 핵심 자료입니다.

*   **Overview of the SPARC physics basis (Nuclear Fusion, 2022)**
    *   *설명:* 고온 초전도 자석을 도입해 크기를 혁신적으로 줄인 SPARC 프로젝트의 물리적·구조적 배경 총망라.
    *   *링크:* [MIT 공식 저장소 PDF 다운로드](https://mit.edu)
*   **The SPARC Toroidal Field Model Coil Program (arXiv)**
    *   *설명:* 극소형 핵융합로의 핵심인 '절연체 없는(No-Insulation) 고자기장 자석'의 핵심 전자기적 원리와 시험 결과 수록.
    *   *링크:* [arXiv PDF 다운로드](https://arxiv.org)
*   **MIT / CFS SPARC & ARC Papers List**
    *   *설명:* 고온 초전도 자석, 저온 냉각 및 구조 설계 관련 MIT/CFS의 핵심 논문들을 모아놓은 오픈 링크 리스트.
    *   *링크:* [공개 PDF 링크 리스트](https://ma2life.org)

---

## 🛠️ 3. 전자공학 엔지니어 관점의 연구 로드맵

### 1단계: 선재 특성 및 거시적 물리 이해
*   **파인만 물리학 강의 3 (제21장):** 초전도 현상을 거대한 파동함수로 해석하는 '거시적 양자 현상' 관점과 조셉슨 효과 빠르게 발췌독 (개념 확립용).
*   **REBCO 선재 파라미터 파악:** 임계 전류 밀도($J_c$), 임계 자기장($B_c$), 임계 온도($T_c$) 간의 비선형적 관계식 정립.

### 2단계: 수치 해석 및 시뮬레이션 (Multiphysics)
*   **COMSOL Multiphysics 활용:** `AC/DC 모듈`(전자기장 해석)과 `Heat Transfer 모듈`(열해석)을 연동하여 무절연(No-Insulation) HTS 코일 내 전류 밀도 및 자기장 분포 모사.

### 3단계: 전력 제어 및 퀜치 보호 시스템 설계
*   **퀜치(Quench) 검출 회로:** 초전도 파괴 시 발생하는 $nV$ 단위의 미세 전압 변화를 감지하는 고속 신호처리 회로 설계.
*   **인터록(Interlock) 회로:** 초전도 자석이 타버리지 않도록 전류를 외부 덤프 저항(Dump Resistor)으로 우회시키는 고전력 스위칭 회로 모델링.
