# YOLO26 Object Detection Results

본 저장소는 YOLO26 모델을 이용한 객체 탐지 실험 결과를 정리한 레포지토리입니다.  

결과 페이지: (https://github.com/schyuks/Pothole_project/blob/main/Pothole.ipynb)

---

## 프로젝트 개요

- 모델: YOLO26m
- 학습 Epoch: 100
- 목적: 객체 탐지 성능 평가 및 결과 시각화
- 프레임워크: Ultralytics YOLO

---

## 폴더 구조


---

## 주요 파일 설명

### 1. yolo26m_epoch_100/best.pt
학습이 완료된 최종 모델 가중치 파일입니다.  
validation 기준 성능이 가장 좋았던 checkpoint입니다.

### 2. yolo26m_epoch_100/args.yaml
학습에 사용된 모든 하이퍼파라미터 설정 파일입니다.

예시:
- 모델 구조
- 이미지 사이즈
- batch size
- optimizer
- epoch 수 등

실험 재현성을 위해 가장 중요한 파일입니다.

### 3. yolo26m_epoch_100/results.csv
Epoch별 학습 로그입니다.

포함 정보:
- precision
- recall
- mAP50
- mAP50-95
- loss 값들

엑셀이나 pandas로 열어서 분석 가능합니다.

### 4. yolo26m_epoch_100/results.png
Epoch에 따른 성능 변화 그래프입니다.

- box loss
- cls loss
- mAP
- precision / recall

---
