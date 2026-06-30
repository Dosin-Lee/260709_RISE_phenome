# 260709 RISE Phenome

RISE 표현체 교육용 Colab 실습 자료입니다. 표현체 분석을 처음 접하는 교육생이 이미지 전처리, 객체 분할, ROI 계측, Naive Bayes, k-means 실습을 순서대로 따라갈 수 있도록 구성했습니다.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Dosin-Lee/260709_RISE_phenome/blob/main/notebooks/RISE_phenotyping_practice.ipynb)

## 교육생 사용 방법

1. 위 **Open In Colab** 버튼을 클릭합니다.
2. Colab이 열리면 우상단 `연결`을 누릅니다.
3. 0장 준비 셀부터 위에서 아래로 실행합니다.
4. 첫 실행에서 패키지를 설치한 뒤 런타임이 재시작되면, 다시 연결한 후 0장 준비 셀부터 한 번 더 실행합니다.
5. 결과 CSV와 모델 파일은 노트북 마지막의 `rise_results.zip` 셀에서 내려받습니다.

## 파일 구조

```text
notebooks/
  RISE_phenotyping_practice.ipynb
assets/
  rise_phenotyping_assets.zip
requirements_rise_phenotyping.txt
```

## 포함 파일

- `notebooks/RISE_phenotyping_practice.ipynb`: 교육생용 Colab 노트북
- `assets/rise_phenotyping_assets.zip`: GitHub/기관망 장애 대비 예제 데이터 묶음
- `requirements_rise_phenotyping.txt`: uv/pip 설치용 의존성 목록

## 실행 환경

- Google Colab CPU 런타임 기준
- GPU 불필요
- 첫 실행 시 인터넷 연결 필요
- 노트북은 `uv`를 우선 사용하고, 실패 시 `pip`로 대체합니다.

## 고정 의존성

교육 당일 PC와 Colab 런타임 차이로 인한 오류를 줄이기 위해 주요 패키지는 정확한 버전으로 설치됩니다. 핵심 버전은 `plantcv==4.11.1`, `numpy==2.2.6`, `scipy==1.15.3`, `opencv-python==4.13.0.92`, `scikit-image==0.26.0`, `scikit-learn==1.9.0`, `pandas==3.0.3`입니다.

이미 열린 Colab 런타임에서 NumPy/SciPy 관련 import 오류가 발생하면 `런타임 > 런타임 다시 시작`을 실행한 뒤 0장 준비 셀부터 다시 실행합니다.

## 데이터 출처

예제 데이터는 Danforth Center PlantCV 공개 튜토리얼 자료를 사용합니다. 노트북에는 2026-06-29 기준 확인한 commit SHA가 고정되어 있습니다.

- PlantCV tutorial data: CC BY 4.0
- simple RGB workflow commit: `6e9c35d736bc31782af3e760096c03f5dbe34049`
- supervised ML commit: `d57501166da0218a388a0f23f681a0117bf1bf76`
- unsupervised ML commit: `4a52eb64edbaa343cc86ab9793e61de28d1dcb5a`
