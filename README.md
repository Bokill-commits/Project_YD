# 🎬 Project_YD | 영상 데이터 수집 자동화 스크립트

Google Colab 환경에서 yt-dlp를 활용해 유튜브 영상을 원하는 화질로 수집할 수 있는 자동화 스크립트입니다.

---

## ⚠️ 주의사항

본 프로젝트는 학습 및 개인적인 용도로 제작되었습니다.

사용 시 YouTube 이용약관 및 저작권 관련 법규를 준수해야 합니다.

저작권이 있는 콘텐츠를 무단으로 다운로드하는 행위는 법적 문제를 초래할 수 있습니다.

본 프로젝트의 오용에 대한 책임은 사용자에게 있습니다.

##

## ⚠️ Disclaimer

This project is intended for educational and personal use only.

Please ensure that you comply with YouTube's Terms of Service and applicable copyright laws when using this tool.

Downloading copyrighted content without permission may violate laws and platform policies.

The author is not responsible for any misuse of this project.

---

## 📌 프로젝트 특징

- 유튜브 영상 정보 자동 분석
- 선택 가능한 화질 리스트 제공
- 다운로드 진행률 실시간 출력
- 선택한 화질로 자동 다운로드
- PC로 바로 다운로드 지원 (Google Colab)

---

## 🛠️ 기술 스택

| Language | Tools | Core |
|-----------|------|------|
| Python | Google Colab | yt-dlp / ffmpeg |

---

## 🧠 핵심 로직

- yt-dlp를 활용하여 영상 메타데이터(title, duration, formats 등) 추출
- 사용 가능한 해상도(height)를 기준으로 비디오 스트림 필터링
- 비디오 스트림과 오디오 스트림을 선택하여 병합 (ffmpeg 활용)
- progress_hook을 통해 다운로드 진행률을 실시간으로 출력
- 다양한 해상도 옵션을 사용자에게 제공하기 위해 포맷 정보를 정렬 및 가공

---

## ⚙️ 실행 방법

1. Google Colab 실행
2. 라이브러리 환경 설치
3. 메인 코드 실행
4. 데이터 수집 할 유튜브 URL 입력
5. 원하는 화질 선택 → 자동 다운로드

---

## 🔄 개선 방향

- GUI 인터페이스 추가 (Streamlit)
- 다중 영상 병렬 다운로드
- 자막 다운로드 기능
- 영상 포맷(mp3 변환) 지원
