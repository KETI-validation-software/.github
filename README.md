# .github
Validation Software tool for testing request/response messages

# Project Structure

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
│   ├─ json_checker.py         # JSON 스키마 검증
│   ├─ validators/             # 검증 모듈
│   │   ├─ base_validator.py
│   │   ├─ system_validator.py
│   │   └─ platform_validator.py
│   └─ reports/                # 리포트 생성 모듈
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
├─ ui/                         # GUI
│   ├─ runner_gui/             # 시험 진행 GUI (정수인 담당)
│   │   └─ ...
│   └─ info_gui/               # 시험 정보 GUI (장예진 담당)
│       └─ ...
│
├─ assets/                     # 리소스
│   ├─ fonts/
│   │   ├─ NamuGothic.ttf
│   │   └─ NamuGothic.pkl
│   └─ images/
│       └─ 버튼 이미지들
│
└─ tests/                      # 단위/통합 테스트
    ├─ test_validators.py
    ├─ test_api.py
    └─ test_ui.py
```
