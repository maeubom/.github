# 감정 분석 기반 상담 서비스

## 1. 프로젝트 개요
사용자의 영상과 음성을 분석하여 감정 상태를 파악하고, 이에 따른 맞춤형 콘텐츠(명언, 음악 등)를 제공하는 서비스입니다.

## 2. 주요 기능

### 2.1 프론트엔드 인터페이스

#### 2.1.1 영상 녹화 기능
- **우선순위**: High
- 사용자의 영상과 음성을 동시에 녹화
- 실시간 영상 피드백 제공
- 녹화 품질 설정 기능

#### 2.1.2 녹화 제어 기능
- **우선순위**: High
- 일시정지 기능
- 녹화 종료 기능
- 녹화 취소 기능

#### 2.1.3 분석 진행 화면
- **우선순위**: Medium
- 분석 진행률 표시
- 취소 옵션 제공
- 로딩 애니메이션

#### 2.1.4 분석 결과 화면
- **우선순위**: High
- 감정 분석 요약 대시보드
  - 주요 감정 상태 그래프
  - 시간별 감정 변화 추이
- 추천 콘텐츠 섹션
  - 상황에 적합한 명언/글귀 표시
  - 음악 추천 또는 생성된 음악 재생
- 저장 및 공유 기능

#### 2.1.5 갤러리 기능
- **우선순위**: Medium
- 과거 분석 결과 목록 표시
- 결과별 상세 보기
- 결과 삭제 기능

### 2.2 백엔드 기능

#### 2.2.1 영상 분석 처리 (Transformer.js)
- **우선순위**: High
- 실시간 감정 데이터 추출
- 감정 데이터 정규화 및 가공
- 음성의 텍스트 변환 (STT)

#### 2.2.2 콘텐츠 생성/추천 시스템
- **우선순위**: Medium
- 감정 기반 음악 추천/생성
- 상황별 적절한 명언 선택
- 개인화된 피드백 생성

#### 2.2.3 데이터 저장 및 관리
- **우선순위**: Medium
- 사용자 세션 관리
- 분석 결과 저장
- 데이터 백업 및 복구

## 3. 기술 스택

### 3.1 프론트엔드
- **Framework**: React
- **상태관리**: (추가 필요)
- **UI 라이브러리**: (추가 필요)

### 3.2 백엔드
- **Framework**: Python (FastAPI)
- **Database**: MongoDB


### 3.3 AI 모델
1. 사진 감정 인식: `motheecreator/vit-Facial-Expression-Recognition` (Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral)
2. 음성-텍스트 변환: `SungBeom/stt_kr_conformer_ctc_medium`
3. 텍스트 요약: `lcw99/t5-base-korean-text-summary` / `csebuetnlp/mT5_multilingual_XLSum`
4. 텍스트 감정 인식: `lxyuan/distilbert-base-multilingual-cased-sentiments-student`
5. 음악 추천/생성: `facebook/musicgen-small`
6. 이미지 생성: `runwayml/stable-diffusion-v1-5`

### 기여자
<h3 align="center">🚀프로젝트 기간</h3>
  <p align="center">2024.10.28 ~ 11.02</p>
  <br>
  <h3 align="center">🚀기여자</h3>
  <br>
  <table align="center">
    <tr>
       <td align="center">
        <strong align="center">김지원</strong><br>
        <img src="https://avatars.githubusercontent.com/JJiwonn" width="100" height="100"><br>
        <a href="https://github.com/JJiwonn">GitHub</a>
        <strong align="center">김화연</strong><br>
        <img src="https://avatars.githubusercontent.com/KHY90" width="100" height="100"><br>
        <a href="https://github.com/KHY90">GitHub</a>
                <strong align="center">신상범</strong><br>
        <img src="https://avatars.githubusercontent.com/sashin92" width="100" height="100"><br>
        <a href="https://github.com/sashin92">GitHub</a>
                <strong align="center">조수현</strong><br>
        <img src="https://avatars.githubusercontent.com/chosuhyeon0812" width="100" height="100"><br>
        <a href="https://github.com/chosuhyeon0812">GitHub</a>
      </td>