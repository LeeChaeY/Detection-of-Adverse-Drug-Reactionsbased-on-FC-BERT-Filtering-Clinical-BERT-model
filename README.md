# Detection-of-Adverse-Drug-Reactionsbased-on-FC-BERT-Filtering-Clinical-BERT-model

## FC-BERT (Filtering Clinical BERT)
FC-BERT 알고리즘 기반의 필터링을 활용한 ADE(Adverse Drug Event) 분류 예측
> 자발적 부작용 보고제도의 낮은 데이터를 보완하기 위해 소셜미디어 데이터로부터 약물 부작용 표현을 탐지하기 위한 방법을 제시한다. 
> 리뷰데이터에서 목표 약물에 대한 부작용 표현을 추출하는 이전 연구에서는 약물을 복용하기 전의 증상이나 
> 목표약물이 아닌 다른 약물에 대한 부작용 표현을 제거하지 못한다는 한계점이 있다. 이런 한계점을 보완하기 위해서 
> SPARK-NLP에서 제공하는 4개의 모델과 단계의 필터링을 활용하여 ADE 말뭉치의 ADE 유무를 판단하는 알고리즘을 개발하였다. 
> 제안하는 알고리즘은 BiLSTM-CNNChar 구조의 Clinical BERT를 기반으로 필터링을 더하여 
> 기존 연구에서 해결하지 못한 약물 복용 전 증상이나 다른 약물의 부작용 표현을 제거함으로써 
> 보다 더 정확하게 약물 부작용 표현을 탐지할 수 있다.
</br>

## 데이터
우리 모델의 성능을 검증하기 위한 데이터로 ADE Corpus V2 데이터를 활용하였다. 
ADE Corpus v2 데이터는 MEDLINE 데이터베이스에 접근가능한 자유 검색 엔진인 
PubMed에서 수집한 23,516개의 ADE 말뭉치로 구성되어있다. 데이터는 
https://github.com/trunghlt/AdverseDrugReaction/tree/master/ADE-Corpus-V2 에서 다운로드 받을 수 있다.
<br></br> 

## 알고리즘

<br></br>

## 코드
.ipynb: 코드의 구성은 다음과 같다.
+ ADE Corpus V2 데이터에 ADE 분류 기반의 약물 부작용 탐지 모델 구축
+ ADE Classifier 파이프라인 모델을 적용하는 기본 모델과 FC-BERT를 비교 실험한 성능 평가 및 NER 결과 시각화
