## Description
AI-Hub 꿀벌 질병 데이터를 YOLOv5 프레임워크를 활용하여 벌의 상태(유충 및 성충의 정상 상태와 질병 상태)를 탐지하고 분류하는 모델을 학습합니다. `AI-Hub -> COCO -> YOLO` 형식으로 변환하여 활용합니다.
## Requirements
본 프로젝트는 **Tesla V100 32GB** 환경에서 작성 및 테스트 되었습니다.
```
pip install -r requirements.txt
```
## Dataset
- AI-Hub에서 제공하는 `꿀벌 질병 데이터셋`을 사용합니다.
- 데이터는 `YOLOv5` 학습 형식에 맞게 변환되어 사용됩니다.
### 클래스
```
1. 유충_정상
2. 유충_응애
3. 유충_석고병
4. 유충_부저병
5. 성충_정상
6. 성충_응애
7. 성충_날개불구바이러스감염증
```
### 폴더 구조
```
/dataset
  ├── images/
  │   ├── train/*.jpg
  │   ├── val/*.jpg
  │   └── test/*.jpg
  └── labels/
      ├── train/*.txt
      ├── val/*.txt
      └── test/*.txt
```