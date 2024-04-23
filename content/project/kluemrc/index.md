---
title: Open-Domain Question Answering
summary: 주어진 지문을 이해하고, 질문에 대한 적절한 답변을 추론하는 Retriever-Reader 모델 개발
date: '2024-02-22T00:00:00Z'


image:
    focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    url: https://github.com/boostcampaitech6/level2-nlp-mrc-nlp-03
---
> 부스트캠프 AI Tech 교육 과정 내 프로젝트 / 2024.02.07~2024.02.22
* **관련 기술:** RAG, ColBERT, BM25, RAGatouille, transformers
* **개요:** 주어진 지문을 이해하고, 질문에 대한 적절한 답변을 추론하는 Retriever-Reader 모델 개발
* **역할:**
    * Retriever 성능 개선
        * 쿼리-문서 간의 유사도 계산을 토큰(단어) 단위로 수행하여 <span style='color:red'><u>**보다 정확하게 지문을 검색**</u></span>할 수 있도록 ColBERT 구현
        * Hard Negative Sampling 과정이 학습 파이프라인에 포함된 RAGatouille 라이브러리를 사용하여 ColBERT 학습 성능 극대화
* **성과 및 배운점:**
    * <span style='color:red'><u>**리더보드 1위 (최종)**</u></span>: EM 72.00 / F1: 82.41