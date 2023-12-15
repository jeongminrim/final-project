# Brain Tumor Classification Project

## Overview
이 프로젝트는 MRI 이미지를 기반으로 한 brain tumor의 분류를 목표로 합니다. Dataset은 pituitary_tumor, no_tumor, meningioma_tumor, glioma_tumor의 네가지 범주를 포함하고 있습니다. scikit-learn library에서 제공하는 Random Forest Classifier를 활용하여 수행하였습니다.

## Dataset
데이터셋은 MRI 이미지를 기반으로 하며, training, testing 폴더로 구성되어 있습니다. 각 폴더에는 해당 종양 범주의 MRI를 담은 하위 폴더들이 존재합니다.

## Algorithm
Random Forest Classifier를 사용하였습니다. Random Forest는 복잡한 데이터셋을 처리하는 데 효과적입니다.

## Hyperparameters
Random Forest Classifier의 Hyperparameters는 최적의 성능을 위해 조정하였습니다:

- Bootstrap: False
- Max Features: 'sqrt'
- Min Samples Leaf: 1
- Min Samples Split: 3
- Estimators 수: 100
- 랜덤 시드: 42

## 결과
분류 결과의 정확도는 노트북의 끝에 출력됩니다. 이 정확도 점수는 뇌종양 분류 모델의 성능을 평가하는 지표로 사용됩니다.

코드를 탐색하고 실험 또는 개선을 위해 코드를 조정하십시오. 문제가 발생하거나 제안 사항이 있는 경우 GitHub 리포지토리에서 이슈를 작성해 주세요.
