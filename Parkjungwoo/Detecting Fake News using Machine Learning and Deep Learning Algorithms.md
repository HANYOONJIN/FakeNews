 # Detecting Fake News using Machine Learning and Deep Learning Algorithms
 
* 논문 저자 정보 (이름, 소속)
 - Abdullah-All-Tanvir, Ehesas Mia Mahir, Saima Akhter, Mohmmad Rezwanul Huq
   East West University, Bangladesh 
   
* 논문에서 가짜뉴스를 검출하려는 뉴스 종류
 - 트위터에서의 뉴스(소셜미디어)
   정부문제, 세계 유행주제, 정신적 학대, 도시의 전설, 재난사건 등의 여러종류의 트윗
 
* 논문에서 정의하고 있는 가짜뉴스
 - 가짜, 실수, 사실이 아닌 트윗
 
* 논문에서 학습에 사용되는 데이터
  Chile Earthquake 2010 Dataset, 데이터양 : 20,360개의 데이터
  
  - 데이터 전처리 방법
   1. 데이터셋 처리
    1.1 데이터 집합을 H : 가짜, 나쁜의도를 가진 트윗 , N : 실수, 나쁜의도를 가지지않은 트윗으로분류
    1.2 트윗의 단어길이를 분석 : 인증되지 않은 뉴스 컨텐츠가 많은 제목, 단어 및 허구의 진술, 링크, 날짜 또는 표시가 없는 부분
   2. Count Vectors
   3. TF_IDF
    3.1 World Level
    3.2 N-gram Level
    3.3 Character Level
   4. Word Embedding : 단어와 문서를 벡터로 표현
   
  - 개발 관련 구현언어 : Python 3.65.
  -  **(검토자 의견) 데이터 객관성 여부에 대한 검토 의견**  
* 논문에서 사용하는 알고리즘  
  - 사용한 머신러닝 알고리즘 종류
   1. SVM
   2. NaiveBayes
   3. LR (Logistic Regression)
   4. Recurrent Neural Network(RNN)
   5. Long short-term memory
   
  - 학습 방식 : 지도(분류기) + 강화(RNN)
  - 신경망을 사용할 경우 네트워크 내용
    LSTM 이용 : 임베디드레이어, 숨겨진레이어, 입/출력 레이어, Sigmoid 활성화 함수와 glorot_nomal사용 
    
  - **(검토자 의견) 알고리즘이 논문에서 정의하는 가짜 뉴스를 검출하기에 적합한지 검토 의견** 
* **오픈소스 공개 여부** 
* 논문의 평가
  - 논문에서 주장하는 내용 
  - 논문 결과 (정량적 또는 정성적 결과)
    SVM과 Naive Bayes 분류기 다른알고리즘보다 우수
    제안하는 4가지의 벡터 (Count Vector, World Level Vectors, N-gram Vectors, Character Level Vectors) 비교 분석

|--|NaiveBayes|---|
|특징벡터|73%
|카운터벡터|75%
  - **(검토자 의견) 논문 결과에 대한 객관성에 대한 검토의견** 

* 관련연구: 논문에서 기술하는 관련 연구 부분 중 검토필요가 있는 것은 일반 논문의 검토와 같은 수준의 논문 리뷰를 하는 것으로 
확장하기 위한 것으로 규정
