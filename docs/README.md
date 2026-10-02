# 프로젝트 문서

개발 과정에서 다음 문서를 작성합니다.

- [`requirements.md`](requirements.md): SDR 기능 초안, HW, FW와 PC SW 스펙
- `architecture.md`: 시스템 구성, 담당 범위, 데이터 흐름
- [`interface.md`](interface.md): I/Q 비트 폭, 순서, 샘플률, 캡처 파일 형식
- [`bringup.md`](bringup.md): Linux 펌웨어로 보드를 구동해 PC에서 IQ를 받기까지의 단계별 절차, 복구 방법
- [`guide/bringup-guide.pdf`](guide/bringup-guide.pdf): 위 절차의 세부 작업판(인쇄용 기록표 포함). HTML 원본을 고친 뒤 Chrome으로 다시 PDF를 만듭니다
- [`guide/custom-sdr-plan.pdf`](guide/custom-sdr-plan.pdf): PL(RTL)부터 PS(PetaLinux)까지 직접 만드는 개발 계획. 참고 설계에서 추출한 보드 정보, 단계별 작업, 확인 필요 항목 포함
- [`guide/axi-ad9361-guide.pdf`](guide/axi-ad9361-guide.pdf): ADI `axi_ad9361`(fmcomms2/zed 포팅)과 ADI Linux로 보드를 직접 빌드해 PC까지 IQ를 받는 가이드와 8주 일정. HTML 원본을 고친 뒤 Chrome으로 다시 PDF를 만듭니다

참고 자료는 `references/`에 둡니다.

- [`references/matlab-korea-videos.md`](references/matlab-korea-videos.md): 로드맵 단계별 MATLAB Korea 참고 영상

아직 확정되지 않은 사양은 미정으로 표시합니다.
시험 결과에는 소스 버전, 장비와 설정, 수행 절차, 관찰 결과를 기록합니다.
