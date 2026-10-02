# SDR 팀 프로젝트

Zynq와 AD9361 기반 보드를 활용해 SDR 수신 시스템을 개발하는 팀 프로젝트입니다.
현재는 저장소의 초기 구조를 준비하는 단계이며, 보드 구동과 기능 구현은 아직 검증하지 않았습니다.

## 프로젝트 구성

| 폴더 | 용도 |
| --- | --- |
| `vivado_project/` | FPGA RTL, 핀, 타이밍 제약, Block Design, 프로젝트 생성, 빌드 스크립트 |
| `sw/` | 보드 PS 펌웨어와 PC 수신, 복조 프로그램 |
| `docs/` | 시스템 구성, 데이터 인터페이스, 보드 구동 절차, 시험 결과 |

보드 PS 코드와 PC 프로그램이 추가되면 `sw/firmware/`와 `sw/host/`로 구분합니다.

기능 초안과 초기 목표 스펙은 [SDR 기능 정의서](docs/requirements.md)에 정리합니다.

## 개발 환경

팀에서 아래 항목을 확정한 뒤 실제 사용 버전을 기록합니다.

| 항목 | 상태 |
| --- | --- |
| 보드 모델, 하드웨어 리비전 | OpenSourceSDRLab PlutoSky 7020-SDR (AD9361, PA 포함), 리비전 확인 필요 |
| Vivado 버전 | 2022.2 (PetaLinux 2022.2, ADI 2022_R2와 맞춤) |
| PS 개발 도구, 운영체제 | Linux: 제조사 SD 카드 펌웨어(Pluto 기반), [`docs/bringup.md`](docs/bringup.md) 참고 |
| PC 프로그램 언어, 실행 환경 | Python 3.10+, libiio 0.26, pyadi-iio (`sw/host/`) |
| 기반 HDL, 펌웨어 소스 버전 | 확정 필요 |

## 시작하기

```powershell
git clone https://github.com/eroun99/SDR.git
cd SDR
```

현재는 실행 가능한 FPGA 프로젝트나 프로그램이 없습니다.
기본 프로젝트를 추가할 때 해당 폴더에 빌드, 실행 방법을 함께 기록합니다.
파일 참조에는 가능한 한 상대경로를 사용하고, 팀원이 새로 내려받은 환경에서도 빌드되는지 확인합니다.

## 협업 방법

1. 작업 내용과 완료 조건을 Issue에 정합니다.
2. 최신 `main`에서 작업 브랜치를 만듭니다.
3. 기능을 개발하고 검증 결과를 기록합니다.
4. 변경을 커밋하고 GitHub에 올립니다.
5. Pull Request로 팀원 검토 후 `main`에 합칩니다.

예시 브랜치 이름: `feature/rx-ddc`, `feature/ps-streaming`, `feature/host-demod`.

커밋 전에는 `git status`와 변경 내용을 확인합니다.
Pull Request에는 변경 이유, 확인 방법, 다른 파트에 미치는 영향을 적습니다.
보드에서 함께 동작한 버전은 사용한 소스 버전과 시험 조건을 함께 남깁니다.

## 파일 관리

- RTL, XDC, 필요한 `.xpr`, `.bd`, `.xci`, Tcl 및 사용자 IP 소스는 관리 대상입니다.
- Vivado 캐시와 빌드 결과는 `.gitignore`로 제외합니다.
- 사용자 소스는 생성, 캐시 폴더 안에 두지 않습니다.
- 큰 I/Q 녹화 파일과 배포용 빌드 결과는 별도 보관하고 위치를 문서에 기록합니다.
- `.gitignore`는 이미 Git이 추적 중인 파일을 자동으로 제거하지 않습니다.
- 기반 프로젝트를 가져올 때 원본 라이선스와 출처를 유지합니다.
