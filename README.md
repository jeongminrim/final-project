# Brain Tumor Classification Project

## Overview
이 프로젝트는 MRI 이미지를 기반으로 한 brain tumor의 분류를 목표로 합니다. Dataset은 pituitary_tumor, no_tumor, meningioma_tumor, glioma_tumor의 네가지 범주를 포함하고 있습니다. scikit-learn library에서 제공하는 Random Forest Classifier를 활용하여 수행하였습니다.

## Dataset
데이터셋은 MRI 이미지를 기반으로 하며, training, testing 폴더로 구성되어 있습니다. 각 폴더에는 해당 종양 범주의 MRI를 담은 하위 폴더들이 존재합니다. 이미지는 모델 훈련을 용이하게 하기 위해 전처리되고 64x64 픽셀로 크기를 조정했습니다.

## Algorithm
Random Forest Classifier를 사용하였습니다. Random Forest는 복잡한 데이터셋을 처리하는 데 효과적입니다. Random Forest는 분류, 회귀 분석 등에 사용되는 앙상블 학습 방법의 일종으로, 훈련 과정에서 구성한 다수의 결정 트리로부터 부류(분류) 또는 평균 예측치(회귀 분석)를 출력함으로써 동작합니다.

## Hyperparameters
Random Forest Classifier의 Hyperparameters는 최적의 성능을 위해 조정하였습니다:

- Bootstrap: False
- Max Features(최적의 분할을 위해 고려할 최대 feature 개수): 'sqrt'
- Min Samples Leaf(리프노드가 되기 위해 필요한 최소한의 샘플 데이터수): 1
- Min Samples Split(노드를 분할하기 위한 최소한의 샘플 데이터수): 3
- Estimators 수(결정트리의 개수): 100
- 랜덤 시드: 42

여기에서 Min Samples Leaf, Min Samples Split는 과적합을 제어하는데 사용됩니다.

## Results
분류 결과의 정확도는 노트북의 끝에 출력됩니다. 이 정확도 점수는 Brain Tumor Classification model의 성능을 평가하는 지표로 사용됩니다.

