# Project Structure

<p align="center">
  <img src="https://github.com/user-attachments/assets/ff7da07d-f66c-4373-9a35-b12f75e220a6" alt="<프로젝트명> Banner" width="100%" />
</p>

<h1 align="center">🧠 <프로젝트명> · <한줄 슬로건></h1>

<p align="center">
  <!-- Release -->
  <a href="https://github.com/<org>/<repo>/releases">
    <img src="https://img.shields.io/github/v/release/<org>/<repo>?label=release" />
  </a>

  <!-- Python 버전 -->
  <img src="https://img.shields.io/badge/python-3.9%20-blue" />

  <!-- CI (GitHub Actions) -->
  <a href="https://github.com/<org>/<repo>/actions">
    <img src="https://img.shields.io/github/actions/workflow/status/<org>/<repo>/tests.yml?label=ci" />
  </a>

  <!-- Coverage -->
  <a href="https://codecov.io/gh/<org>/<repo>">
    <img src="https://img.shields.io/codecov/c/github/<org>/<repo>?label=coverage" />
  </a>

  <!-- Custom 기능 배지 -->
  <img src="https://img.shields.io/badge/Webhook-supported-brightgreen" />
  <img src="https://img.shields.io/badge/PyInstaller-ready-orange" />
  <img src="https://img.shields.io/badge/GUI-PyQt5-ff69b4" />
  <img src="https://img.shields.io/badge/Report-PDF%20Export-success" />
</p>

```text
validation-tool/
├─ requirements.txt
├─ config/                     # 설정 관련
│   ├─ CONSTANTS.py
│   ├─ config.txt
│   └─ key0627/                # 인증 키 파일
│
├─ core/                       # 공통 엔진 / 도메인
│   ├─ functions.py            # 공통 유틸
│   └─ json_checker.py         # JSON 스키마 검증
│
├─ api/                        # API 서버/웹훅
│   ├─ api_server.py
│   ├─ webhook_server.py
│   └─ routes/                 # 엔드포인트별 처리
│
├─ specs/                      # 명세 (Request/Response + Schema)
│   ├─ bio/
│   │   ├─ bioRequest.py
│   │   ├─ bioSchema.py
│   │   └─ requests/           # JSON 예제
│   ├─ security/
│   │   ├─ securityRequest.py
│   │   ├─ securitySchema.py
│   │   └─ requests/
│   └─ video/
│       ├─ videoRequest.py
│       ├─ videoSchema.py
│       └─ requests/
│
│
├─ assets/                     # 리소스
│   ├─ fonts/
│   │   ├─ NamuGothic.ttf
│   │   └─ NamuGothic.pkl
│   └─ images/
│       └─ 버튼 이미지들
│
├─ launcher_GUI.py            # 장예진 담당
├─ platformVal_all.py         # 정수인 담당
├─ systemVal_app.py           # 정수인 담당
└─ 
```
