# 뇌종양 분류 프로젝트

## 프로젝트 개요
이 프로젝트는 MRI 이미지를 기반으로 한 뇌종양의 분류를 목표로 합니다. 데이터셋은 양성 종양, 악성 종양, 피뇌하선 종양, 그리고 종양이 없음의 다양한 범주를 포함하고 있습니다. 프로젝트는 scikit-learn 라이브러리에서 제공하는 랜덤 포레스트 분류기를 활용하여 이루어집니다.

## 데이터셋
데이터셋은 MRI 이미지를 기반으로 하며, 훈련 및 테스트 폴더로 구성되어 있습니다. 각 폴더에는 해당 종양 클래스의 MRI를 담은 하위 폴더들이 존재합니다.

## 알고리즘 선택
프로젝트에서는 랜덤 포레스트 분류기를 사용하였습니다. 랜덤 포레스트는 앙상블 학습 방법으로, 복잡한 데이터셋을 처리하는 데 효과적입니다.

## 하이퍼파라미터
랜덤 포레스트 분류기의 하이퍼파라미터는 최적의 성능을 위해 조정되었습니다. 선택된 하이퍼파라미터는 다음과 같습니다:

- Bootstrap: False
- Max Features: 'sqrt'
- Min Samples Leaf: 1
- Min Samples Split: 3
- Estimators 수: 100
- 랜덤 시드: 42

## 프로젝트 구조
### 파일 설명
- **brain_tumor_classification.ipynb**: Jupyter Notebook으로 데이터셋 로딩, 이미지 전처리, Random Forest 분류기 훈련, 모델 성능 평가에 대한 코드를 포함하고 있습니다.
- **README.md**: 이 파일은 프로젝트에 대한 개요를 제공하며 데이터셋, 알고리즘 선택, 하이퍼파라미터, 결과 재현에 대한 지침을 설명합니다.

### 재현 지침
1. GitHub 리포지토리를 복제합니다: `git clone https://github.com/your-username/brain-tumor-classification.git`
2. 프로젝트 디렉토리로 이동합니다: `cd brain-tumor-classification`
3. Jupyter Notebook을 실행합니다: `jupyter notebook brain_tumor_classification.ipynb`
4. 노트북에서 데이터를 로드하고 모델을 훈련하며 정확성을 평가하는 단계를 따릅니다.

## 결과
훈련된 Random Forest 분류기의 테스트 데이터셋 정확도는 노트북의 끝에 출력됩니다. 이 정확도 점수는 뇌종양 분류 모델의 성능을 평가하는 지표로 사용됩니다.

코드를 탐색하고 실험 또는 개선을 위해 코드를 조정하십시오. 문제가 발생하거나 제안 사항이 있는 경우 GitHub 리포지토리에서 이슈를 작성해 주세요.
