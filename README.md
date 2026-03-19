# linux-kernel-tracing 🐧

> **Learning Linux Kernel internals and debugging using TRACE32 & ftrace based on v6.1**

이 저장소는 리눅스 커널의 핵심 구조를 분석하고, 실무에서 필수적인 **TRACE32** 및 **ftrace** 디버깅 기술을 학습한 기록을 담고 있다. 시스템 반도체 및 자동차 SW 분야의 임베디드 시스템 소프트웨어 엔지니어를 목표로 하며, 커널 v6.1 기반의 실전 분석 역량을 쌓는 것을 목적으로 한다.

---

## 🛠 Tech Stack & Tools
* **Kernel Version:** Linux v6.1 (Mainline)
* **Architecture:** Armv8-A (64-bit)
* **Debugging Tools:** TRACE32 Simulator, Crash-Utility, ftrace
* **Languages:** C, Shell Script

---

## 📂 Repository Structure

각 코스별 핵심 개념 정리와 실습 로그를 디렉토리별로 관리

### [01] Intro & Overview
* 리눅스 커널 전체 구조 및 시스템 소프트웨어 생태계 이해
* 최신 커널(v6.1)의 변화 및 학습 로드맵 설정

### [02] Debugging Basic
* `printk`, `dump_stack()`, `sysrq` 활용법
* ftrace 기초: 트레이서 설정 및 메시지 분석 방법

### [03] Advanced Debugging (Real-world)
* **TRACE32** 시뮬레이터 활용 메모리 덤프 분석
* Crash-Utility를 이용한 커널 패닉(Kernel Panic) 디버깅 케이스 스터디

### [04] Process Management
* `struct task_struct` 및 `current` 매크로 심층 분석
* 프로세스 생성/종료 흐름 트레이싱 및 컨텍스트 스위칭 이해

### [05] Interrupt Handling
* IRQ 서브시스템 구조 및 Armv8 GIC 인터럽트 흐름
* 인터럽트 핸들러 등록 및 실행 경로 디버깅

### [06] Interrupt Bottom Half
* 인터럽트 후반부 처리 기법: `Softirq`, `Tasklet`, `Threaded IRQ`
* 실전 디바이스 드라이버 최적화 전략 학습

### [07] Workqueue
* 워크큐(Workqueue) 자료구조 분석 및 활용
* 시스템 소프트웨어 관점에서의 비동기 작업 처리 매커니즘

---

## 🚀 Key Learning Points
* **TRACE32 Mastery:** 단순 코드 분석을 넘어 메모리 덤프를 통해 실제 커널의 상태를 가시화하는 능력 배양
* **ftrace Analysis:** 함수 호출 흐름과 실행 시간을 정밀하게 분석하여 성능 병목 지점 파악
* **Low-level Insight:** Armv8 아키텍처 기반 위에서 커널이 하드웨어 인터럽트와 프로세스를 제어하는 원리 습득

---
