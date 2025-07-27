#  GCP Vertex AI AutoML – 꽃 이미지 분류 실습

Google Cloud Platform(GCP)의 Vertex AI를 활용하여  
꽃 이미지 데이터셋을 기반으로 한 이미지 분류 모델을 AutoML로 학습하고 배포하는 실습을 진행하였습니다.

---

##  실습 개요

- **목표**: daisy, rose, tulip, sunflower, dandelion 이미지를 분류하는 모델 생성
- **도구**: GCP Vertex AI Studio - AutoML 이미지 분류
- **데이터**: 총 3,667장의 꽃 이미지 (5종 분류)

---

##  실습 과정

### 1. 데이터셋 업로드 및 라벨링

![dataset](https://github.com/user-attachments/assets/196e157e-e03a-42bf-8cdb-b91398878904)

- 클래스: `daisy`, `dandelion`, `roses`, `sunflowers`, `tulips`
- 총 이미지 수: 3,667장
- 일부 오류는 무시 가능 (공식 가이드라인)

---

### 2. AutoML 모델 학습

![training](https://github.com/user-attachments/assets/57cb0a2d-f358-43e6-9425-08bd2f53921a)

- 기본 AutoML 분류 옵션 사용
- 학습 소요 시간 약 2시간
- 높은 정밀도: `roses` (0.952)

---

### 3. 모델 테스트 및 예측

![test](https://github.com/user-attachments/assets/0edbc7d0-eb87-42ef-9b0c-ee4d3e058cef)

- 테스트 이미지: 빨간 장미
- 예측 결과: **정확히 `roses`로 예측**

---

##  결과 요약

| 항목 | 내용 |
|------|------|
| 분류 대상 | 꽃 이미지 5종 |
| 가장 높은 정확도 | roses (0.952) |
| 실습 방식 | 코드 없이 AutoML UI로 수행 |

---

##  사용 기술

- GCP Vertex AI Studio
- AutoML 이미지 분류
- Google Cloud Storage
- GitHub Markdown
