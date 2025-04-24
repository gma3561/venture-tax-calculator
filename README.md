# 벤처투자 소득공제 시뮬레이터

이 프로젝트는 벤처투자 소득공제에 따른 세금 환급 효과를 시뮬레이션하는 Streamlit 애플리케이션입니다.

## 기능

- 총급여액, 신용카드 사용액, 부양가족 수 등을 입력하여 세금 계산
- 벤처투자 소득공제 전/후 세율 구간 분석
- 벤처투자 소득공제 전/후 환급액 비교
- 투자 효율성 평가

## 로컬에서 실행하기

```bash
# 필요 패키지 설치
pip install -r requirements.txt

# 앱 실행
streamlit run src/venture_caculator.py
```

## Streamlit Cloud에 배포하기

1. [Streamlit Cloud](https://share.streamlit.io/) 웹사이트에 접속
2. GitHub 계정으로 로그인
3. "New app" 버튼 클릭
4. 저장소 선택: 현재 GitHub 저장소 URL 입력
5. 브랜치: `main` 선택
6. 메인 파일 경로: `src/venture_caculator.py` 입력
7. "Deploy!" 버튼 클릭

## 업데이트 내역

- 벤처투자 소득공제 전/후 환급액 비교 기능 추가
- 원천징수 세액 계산 및 정확한 환급액 비교 분석 추가

## 프로젝트 구조

```
venture-tax-calculator/
├── src/                # 소스 코드 폴더
│   └── venture_caculator.py  # 메인 애플리케이션 코드
├── data/               # 데이터 파일 저장 폴더
├── tests/              # 테스트 코드 폴더
├── docs/               # 문서 파일 폴더
├── .streamlit/         # Streamlit 설정 폴더
│   └── config.toml     # Streamlit 테마 설정
├── README.md           # 프로젝트 설명 문서
└── requirements.txt    # 의존성 패키지 목록
```

## 사용 방법

1. 사이드바에서 총급여액, 소득공제 항목 등 정보를 입력하세요.
2. 계산하기 버튼을 클릭하면 결과가 표시됩니다.
3. 세 가지 탭을 통해 세율 구간 분석, 공제 항목 상세, 투자 효율성 평가를 확인할 수 있습니다.

## 설치 및 실행

```bash
# 패키지 설치
pip install -r requirements.txt

# 앱 실행 (루트 디렉토리에서)
streamlit run src/venture_caculator.py
```

## 벤처투자 소득공제율

- 3천만원 이하: 100%
- 3천만원 초과 ~ 5천만원 이하: 70%
- 5천만원 초과: 30%

본 시뮬레이터는 정확한 세금 계산을 보장하지 않으며 참고용으로만 사용하세요.
