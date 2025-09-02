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
