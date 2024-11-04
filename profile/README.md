# 감정 분석 기반 상담 서비스

## 1. 프로젝트 개요
사용자의 영상과 음성을 분석하여 감정 상태를 파악하고, 이에 따른 맞춤형 콘텐츠(명언, 음악 등)를 제공하는 서비스입니다.

### 기여자
<h3 align="center">📹 프로젝트 기간</h3>
<p align="center">2024.10.28 ~ 11.02</p>
<br>
<h3 align="center">📹 기여자</h3>
<br>

<table align="center">
  <tr>
    <td align="center">
      <strong>김지원</strong><br>
      <img src="https://avatars.githubusercontent.com/JJiwonn" width="100" height="100"><br>
      <a href="https://github.com/JJiwonn">GitHub</a>
    </td>
    <td align="center">
      <strong>김화연</strong><br>
      <img src="https://avatars.githubusercontent.com/KHY90" width="100" height="100"><br>
      <a href="https://github.com/KHY90">GitHub</a>
    </td>
    <td align="center">
      <strong>신상범</strong><br>
      <img src="https://avatars.githubusercontent.com/sashin92" width="100" height="100"><br>
      <a href="https://github.com/sashin92">GitHub</a>
    </td>
    <td align="center">
      <strong>조수현</strong><br>
      <img src="https://avatars.githubusercontent.com/chosuhyeon0812" width="100" height="100"><br>
      <a href="https://github.com/chosuhyeon0812">GitHub</a>
    </td>
  </tr>
</table>

<br>
<h3 align="center">📹 프로젝트 아키텍쳐</h3>
<br>

![아키텍처](https://github.com/user-attachments/assets/4608b3f2-83f1-46e4-8447-c1828e9832d2)


<br><br>
## 2. 주요 기능
- 영상 녹화(비디오, 음성)
- 비디오 감정 분석
- 오디오 -> 텍스트로 변환 -> 텍스트 요약 -> 감정 분석
- 비디오와 오디오로 분석된 감정을 바탕으로 명언과 이미지 생성하여 고객에게 전달

## 3. 기술 스택

### 3.1 프론트엔드
- **Framework**: React

### 3.2 백엔드
- **Framework**: Python (FastAPI)

### 3.3 AI 모델
1. 사진 감정 인식: `motheecreator/vit-Facial-Expression-Recognition` (Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral)
2. 음성-텍스트 변환: `openai/whisper-large-v3-turbo`
3. 텍스트 요약: `lcw99/t5-base-korean-text-summary` / `csebuetnlp/mT5_multilingual_XLSum`
4. 텍스트 감정 인식: `Copycats/koelectra-base-v3-generalized-sentiment-analysis`
5. 음악 추천/생성: `facebook/musicgen-small`
6. 명언 생성 : 'facebook/opt-350m'
7. 이미지 생성: `stabilityai/stable-diffusion-xl-base-1.0`

## 4. 비기능적 요구사항

### 4.1 성능 요구사항
- 영상 처리 지연시간: 최대 2초
- 동시 사용자 처리: 최소 100명
- 데이터 저장 용량: 사용자당 1GB

### 4.2 보안 요구사항
- 사용자 데이터 암호화
- 안전한 인증 시스템
- 개인정보 보호 준수

### 4.3 사용성 요구사항
- 직관적인 UI/UX
- 반응형 디자인
- 다국어 지원 (한국어/영어)
