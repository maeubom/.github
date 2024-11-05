# 감정 분석 기반 상담 서비스

## 1. 프로젝트 개요
사용자의 영상과 음성을 분석하여 감정 상태를 파악하고, 이에 따른 맞춤형 콘텐츠(명언, 음악 등)를 제공하는 서비스입니다.

---
<h3>📹 프로젝트 기간</h3>
<p>2024.10.28 ~ 11.05</p>
<br>
<h3>📹 기여자</h3>
<br>

<table>
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
  </tr>
</table>

<br>
<h3>📹 프로젝트 아키텍쳐</h3>
<br>

![아키텍처](https://github.com/user-attachments/assets/4608b3f2-83f1-46e4-8447-c1828e9832d2)

<h3>📹 협업 툴</h3>

- [마음:봄 노션](https://www.notion.so/AI-X-4-4-12d7de0d6eed806da798e6569ecaf382)

- [마음:봄 피그마](https://www.figma.com/design/rWwqKUNTd9QpeSXNovrSoH/%EB%A7%88%EC%9D%8C%3A%EB%B4%84-%EB%94%94%EC%9E%90%EC%9D%B8?node-id=0-1&node-type=canvas&t=hxxE1HxAkuHNLZpW-0)

- [마음:봄 PPT](https://www.canva.com/design/DAGVN02EJC0/vHuMe6R5s6j1BkY2YD_52g/edit)

- [마음:봄 Wiki](https://github.com/maeubom/.github/wiki/%EB%A7%88%EC%9D%8C:%EB%B4%84-(%EB%8B%B9%EC%8B%A0%EC%9D%98-%EB%A7%88%EC%9D%8C%EC%9D%84-%EB%93%A4%EC%97%AC%EB%8B%A4%EB%B4%85%EB%8B%88%EB%8B%A4.))
  
<br>

## 2. 주요 기능
- 영상 녹화(비디오, 음성)
- 비디오 감정 분석
- 오디오 -> 텍스트로 변환 -> 텍스트 요약 -> 감정 분석
- 비디오와 오디오로 분석된 감정을 바탕으로 명언과 이미지 생성하여 고객에게 전달

## 3. 기술 스택
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD300?style=for-the-badge&logo=huggingface&logoColor=black)
![Transformers](https://img.shields.io/badge/Transformers-FFD300?style=for-the-badge&logo=huggingface&logoColor=black)
![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white)
![Canva](https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white)
![nVIDIA](https://img.shields.io/badge/cuda-000000.svg?style=for-the-badge&logo=nVIDIA&logoColor=green)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101)
![Visual Studio](https://img.shields.io/badge/Visual%20Studio-5C2D91.svg?style=for-the-badge&logo=visual-studio&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white)



### 3.1 AI 모델
1. 사진 감정 인식: `motheecreator/vit-Facial-Expression-Recognition` (Angry, Disgust, Fear, Happy, Sad, Surprise, Neutral)
2. 음성-텍스트 변환: `openai/whisper-large-v3-turbo`
3. 텍스트 요약: `lcw99/t5-base-korean-text-summary` / `csebuetnlp/mT5_multilingual_XLSum`
4. 텍스트 감정 인식: `Copycats/koelectra-base-v3-generalized-sentiment-analysis`
5. 음악 추천/생성: `facebook/musicgen-small`
6. 명언 생성 : `facebook/opt-350m`
7. 이미지 생성: `stabilityai/stable-diffusion-xl-base-1.0`
