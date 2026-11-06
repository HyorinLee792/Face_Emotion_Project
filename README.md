
# Face Emotion Analysis

영상 기반 얼굴 표정 및 감정 변화 분석 프로젝트

## 1. Project Overview

본 프로젝트는 딥러닝 기반 얼굴 감정 분류 모델을 활용하여
이미지 및 영상 속 인물의 표정을 분석하는 것을 목표로 합니다.

YOLO를 이용해 얼굴을 검출하고,
EfficientNet-B0를 활용하여 7가지 감정을 분류합니다.

## 2. Tech Stack

- Python
- PyTorch
- EfficientNet-B0
- YOLO
- OpenCV
- MediaPipe
- Scikit-learn
- Pandas
- Google Colab

## 3. Emotion Classification

분류 대상 감정은 총 7가지입니다.

- Angry
- Disgust
- Fear
- Happy
- Neutral
- Sad
- Surprise

EfficientNet-B0 모델의 검증 정확도는 90%입니다.

## 4. Facial Expression Analysis

### Angry Expression

- MediaPipe Blendshapes 기반 특징 추출
- K-means 군집 분석
- 3개 표정 패턴 탐색
- 군집별 특징 비교 및 통계 검정

### Happy Expression

- 입꼬리 움직임 분석
- 눈 찡그림과 입꼬리의 상관관계 분석
- 좌우 입꼬리 차이 분석
- 입꼬리와 입 벌림의 상관관계 분석

## 5. Video Test

YOLO와 EfficientNet을 연결하여 실제 영상에서
1초 간격으로 얼굴 검출 및 감정 예측 테스트를 진행했습니다.

## 6. Project Structure

```text
Face_Emotion_Project/
├── model/
├── results/
├── Emotion_Final.ipynb
├── Face_Emotion_Analysis.ipynb
├── .gitignore
└── README.md
