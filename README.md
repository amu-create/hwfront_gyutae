# AI Trainer

AI Trainer는 Django 기반의 피트니스 웹 애플리케이션입니다. 사용자에게 맞춤형 운동 계획, 식단 추천 및 주변 운동 장소 추천 서비스를 제공합니다.

## 기능

- 맞춤형 운동 계획
- 개인화된 식단 추천
- 위치 기반 운동 장소 추천
- 진행 상황 추적

## 기술 스택

- Django 5.2
- Bootstrap
- SQLite (개발)
- HTML/CSS/JavaScript

## 설치 방법

1. 저장소 클론
   ```bash
   git clone https://github.com/amu-create/hwfront_gyutae.git
   cd hwfront_gyutae
   ```

2. 가상 환경 설정
   ```bash
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   ```

3. 의존성 설치
   ```bash
   pip install -r requirements.txt
   ```

4. 마이그레이션 적용
   ```bash
   python manage.py migrate
   ```

5. 서버 실행
   ```bash
   python manage.py runserver
   ```

## 환경 변수 설정 (필수)

보안을 위해 다음과 같이 환경 변수를 설정해야 합니다:

1. `.env.example` 파일을 복사하여 `.env` 파일 생성
   ```bash
   cp .env.example .env
   ```

2. `.env` 파일에서 다음 환경 변수를 설정:
   - `DJANGO_SECRET_KEY`: Django 비밀키
   - `DJANGO_DEBUG`: 디버그 모드 설정 ('True' 또는 'False')
   - `GOOGLE_MAPS_API_KEY`: Google Maps API 키 (Google Cloud Console에서 새로 발급 받아야 함)

## 라이선스

MIT License

## 기여 방법

1. 이 저장소를 포크합니다.
2. 새 브랜치를 생성합니다 (`git checkout -b feature/amazing-feature`).
3. 변경 사항을 커밋합니다 (`git commit -m 'Add amazing feature'`).
4. 브랜치를 푸시합니다 (`git push origin feature/amazing-feature`).
5. Pull Request를 생성합니다.
