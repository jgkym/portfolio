---
title: 문장 내 개체간 관계 추출
summary: 텍스트 임베딩을 개선하여 문장 내 개체 인식 정확도 향상
date: '2024-02-01T00:00:00Z'


image:
    focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    url: https://github.com/boostcampaitech6/level2-klue-nlp-03
---
> 부스트캠프 AI Tech 교육 과정 내 프로젝트 / 2024.01.24~2024.02.01
* **관련 기술:** R-BERT, UniST, PyTorch Lightning, Hydra, transformers, W&B
* **개요:** 텍스트 임베딩을 개선하여 문장 내 인식 정확도 향상
* **역할:**
    * 실험 환경 구축
        * PyTorch Lightning으로 Boilerplate 제작
        * 모델 및 학습 파라미터 변경을 쉽게 하여 팀원들이 <span style='color:red'><u>**다양한 실험을 빠르게**</u></span> 진행할 수 있도록 Hydra 프레임워크 사용
    * 다양한 모델 실험
        * Semantic Typing을 추가하여 텍스트 내에서 <span style='color:red'><u>**개체 인식 성능을 개선**</u></span>시킨 UniST 구현
        * 관계 추출 태스크에서 <span style='color:red'><u>**BERT의 성능을 강화**</u></span>시킨 R-BERT를 구현
        * <span style='color:red'><u>**클래스 불균형 문제를 해소**</u></span>하기 위한 목적으로 객체 탐지 문제에서 주로 쓰이는 Focal Loss를 사용
    * Error Analysis
        * <span style='color:red'><u>**예측 결과를 정성적으로 분석**</u></span>하여 모델에 적절한 피드백을 전달하고자, W&B Callback을 사용해 Confusion Matrix와 Precision-Recall Curve를 모니터링
* **성과 및 배운점:**
    * 관심 대상 주변 마킹을 통한 텍스트 보정으로 개체 인식 효과 개선