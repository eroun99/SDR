# MATLAB Korea 참고 영상

[MATLAB Korea YouTube 채널](https://www.youtube.com/@MATLABKorea/playlists)의 공개 영상 중 로드맵 단계별로 참고할 영상입니다.
MATLAB SDR 병행 트랙(주 1회)에서 사용합니다.

- 조사일: 2026-09-29 (플레이리스트 97개, 영상 약 960개 검토)
- 영상 제목은 채널에 올라온 그대로 적었습니다.
- 채널에 해당 주제 영상이 없는 단계는 "없음"으로 표시하고 다른 자료로 진행합니다.

## P0 환경·RF 기초 (W01–W02)

복소 기저대역, IQ, Welch PSD, 첫 루프백

| 영상 | 활용 |
| --- | --- |
| [How to Perform FFT in MATLAB](https://youtu.be/8BujT71Mh9c) | FFT 기초 |
| [파워 스펙트럼의 밀도(PSD)와 파워 스펙트럼의 이해](https://youtu.be/yABnRQVKKFA) | Welch PSD |
| [Signal Analyzer 앱으로 간편해진 신호 분석](https://youtu.be/mEsLsAlekaM) | 녹화 IQ 확인 |
| [무선 시스템설계를 위해 MATLAB을 USRP에 연동하기](https://youtu.be/6xVMTFsEnvk) | MATLAB–SDR 송수신 흐름 (장비는 다름) |
| [MATLAB을 활용한 무선 시스템 개발](https://youtu.be/G0d5_M91XAI) | 무선 시스템 개발 흐름 |

## P1–P2 서버·프론트, C·데스크톱 GUI (W03–W08)

FastAPI, React, C 클라이언트, Qt GUI 관련 영상은 없습니다. 보조 자료만 적습니다.

| 영상 | 활용 |
| --- | --- |
| [[MATLAB 기본 강좌] MATLAB에서 Python 코드를 호출하는 방법](https://youtu.be/o3Tv_Y8v01A) | 서버 IQ를 MATLAB으로 교차 검증 |
| [[MATLAB 기본 강좌] Python에서 MATLAB 코드를 호출하는 방법](https://youtu.be/z6jBVq89lgA) | 〃 |
| [[MATLAB 기본 강좌] GitHub를 사용하여 MATLAB에서 소스를 관리하는 방법](https://youtu.be/nkZew4pZWNI) | MATLAB 트랙 결과물 관리 |

## P3 FPGA 기초 (W09–W14)

IP는 cocotb·Icarus 흐름에서 직접 설계하므로, 아래 HDL Coder 영상은 하드웨어 구조와 고정소수점 설계 방식을 익히는 개념 자료로 봅니다.
LiteX, cocotb, Yosys·nextpnr 관련 영상은 없습니다.

| 영상 | 활용 |
| --- | --- |
| [MATLAB을 이용한 FPGA 설계 - 1. MATLAB 및 Simulink를 사용해야 하는 이유](https://youtu.be/Scdo_va-aJU) | 개요 |
| [MATLAB을 이용한 FPGA 설계 - 2. Simulink에서의 하드웨어 모델링](https://youtu.be/zggIQhZGHyU) | 하드웨어 모델링 |
| [MATLAB을 이용한 FPGA 설계 - 3. 효율적인 하드웨어 설계](https://youtu.be/favN7nGJ78g) | 파이프라인, 자원 공유 |
| [FPGA Design Using MATLAB - 4. Conversion to Fixed-Point](https://youtu.be/OKyjIzXIXHs) | numpy 기준 모델과 비트 단위 일치 |
| [MATLAB을 이용한 FPGA 설계 - 5. RTL 생성 및 합성](https://youtu.be/ca-EWzSOYB0) | RTL 생성·합성 흐름 |

## P4 디지털 모뎀 (W15–W20)

Gardner, Costas, 프레임 동기 관련 영상은 없습니다.

| 영상 | 활용 |
| --- | --- |
| [컨벌루션의 정의와 그 중요성](https://youtu.be/USXXFSwx9yA) | RRC·정합필터 기초 |
| [Simulink를 사용한 신호 처리](https://youtu.be/SCPSO95EvzQ) | 신호 처리 모델링 |
| [시스템 식별에 LMS 알고리즘을 적용하는 방법, 파트 1](https://youtu.be/4xgOaMM_h6Q) | 적응 등화기 |

## P5 FPGA 스트리밍 (W21–W25)

Zynq PL 수신 경로, NCO·CIC·DDC

| 영상 | 활용 |
| --- | --- |
| [모델기반 설계로 시작하는 FPGA SoC 프로토타이핑 워크플로우](https://youtu.be/6jrLdfnLJHA) | PS–PL 분할, AXI 데이터 경로 |
| [통신 및 레이더를 위한 FPGA SoC 구현](https://youtu.be/NeyMmyNofXw) | SDR 수신 경로에 IP 삽입 사례 |
| [NR HDL Cell Search 참조 어플리케이션](https://youtu.be/ZPgBbwtH2rE) | 수신기 HDL 구현 레퍼런스 |
| [FPGA 및 Programmable SoC 타겟의 모터 제어 알고리즘 개발](https://youtu.be/isd06T3mi20) | Zynq PS–PL 협업 패턴 (주제는 모터 제어) |

## P6 OFDM (W26–W30)

CP, Schmidl-Cox, 채널 추정·등화, EVM

| 영상 | 활용 |
| --- | --- |
| [5G Toolbox를 사용하여 5G NR 표준 규격 파형을 생성하는 방법](https://youtu.be/NRpNOvYEa1Q) | OFDM 기준 파형, EVM 비교 |
| [Initial Acquisition Procedures in 5G NR](https://youtu.be/tnX-15TILxc) | 타이밍·주파수 동기 |
| [Introduction to Radio Path Analysis Using Ray Tracing & Its Application to Wireless Channels](https://youtu.be/_I8ubLnaPL8) | 다중경로 채널 모델 |
| [6G 기술: MATLAB을 통한 광대역 신호 분석](https://youtu.be/ucpHQjSWA80) | 광대역 신호 분석 |

## P7 앵커·측위 (W31–W34)

TDOA, 2채널 AoA(MUSIC)

| 영상 | 활용 |
| --- | --- |
| [위상 배열이란?](https://youtu.be/AOXyiDoExTw) | 배열 기초 |
| [빔포밍 소개](https://youtu.be/8aZlEgHa7uw) | 빔포밍 기초 |
| [다중 채널 빔포밍이 무선 통신에 유용한 이유](https://youtu.be/0240ijKGQ3Q) | 다중 채널 수신 |
| [Can You Steer Wireless Signals? Principles of Beamforming and MATLAB Demo](https://youtu.be/6wIx7PArAFw) | 빔포밍 데모 |
| [디지털 빔포밍이 레이더에 유용한 이유](https://youtu.be/qZzdvs7xO54) | 디지털 빔포밍 |
| [레이더 원리 이해: FMCW를 이용한 각도 측정](https://youtu.be/-TR7IbQpaXc) | 위상차 기반 각도 추정 |

## P8 AI (W35–W38)

변조 분류 CNN, ONNX 서빙, 도메인 갭

| 영상 | 활용 |
| --- | --- |
| [무선 시스템을 위한 인공지능 개발 개요](https://youtu.be/_eMf8Uo6UYk) | 개요 |
| [무선시스템을 위한 인공지능 적용](https://youtu.be/z6RUp-ytbXA) | 무선 AI 적용 |
| [Introduction to AI Development Examples and Case Studies for Wireless Systems](https://youtu.be/TCzC_iholFI) | 사례 |
| [신호 처리를 위한 딥러닝](https://youtu.be/DkKC2oxHpr8) | 신호 딥러닝 |
| [신호처리 응용프로그램을 위한 데이터 중심 AI (Data-Centric AI)](https://youtu.be/1nDPFaIGal0) | 합성·실측 데이터 차이 |
| [Python과 MATLAB 함께 사용하기 - AI 모델 변환](https://youtu.be/hSM4vjiwNTQ) | PyTorch·ONNX 모델 변환 |
| [압축 기술 사용: 프루닝과 양자화](https://youtu.be/mgPAZCPpSYc) | 모델 경량화 |

## P9 통합 (W39–W40)

| 영상 | 활용 |
| --- | --- |
| [MBD와 CI/CD를 활용하여 다양한 환경의 개발자들과 협업하기](https://youtu.be/p0vb2OFGMlw) | CI/CD 협업 |
