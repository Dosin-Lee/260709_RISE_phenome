# 260709 RISE Phenome

RISE 표현체 교육용 Colab 실습 자료입니다. 표현체 분석을 처음 접하는 교육생이 이미지 전처리, 객체 분할, ROI 계측, Naive Bayes, k-means 실습을 순서대로 따라갈 수 있도록 구성했습니다.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Dosin-Lee/260709_RISE_phenome/blob/main/notebooks/RISE_phenotyping_practice.ipynb)

## 교육생 사용 방법

1. 위 **Open In Colab** 버튼을 클릭합니다.
2. Colab이 열리면 우상단 `연결`을 누릅니다.
3. 0장 준비 셀부터 위에서 아래로 실행합니다.
4. 결과 CSV와 모델 파일은 노트북 마지막의 `rise_results.zip` 셀에서 내려받습니다.

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

## 데이터 출처

예제 데이터는 Danforth Center PlantCV 공개 튜토리얼 자료를 사용합니다. 노트북에는 2026-06-29 기준 확인한 commit SHA가 고정되어 있습니다.

- PlantCV tutorial data: CC BY 4.0
- simple RGB workflow commit: `6e9c35d736bc31782af3e760096c03f5dbe34049`
- supervised ML commit: `d57501166da0218a388a0f23f681a0117bf1bf76`
- unsupervised ML commit: `4a52eb64edbaa343cc86ab9793e61de28d1dcb5a`
