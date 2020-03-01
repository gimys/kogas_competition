# 한국가스공사 빅데이터 공모전 정리  
## 1. 공모전 정보
![공모전](https://github.com/gimys/kogas_competition/blob/master/%EA%B3%B5%EB%AA%A8%EC%A0%84.jpg)
## 2. 공모전 목표
1. 한국가스공사 가스생산기지에서 측정한 시계열 데이터 중 1년치 제공  
2. 각 팀에서 분석 목표를 자체적으로 설정하고 해당 목표에 달성하기 위한 알고리즘을 개발
## 3. 공모전 결과
- 제안서 작성, 데이터 분석, 머신러닝, 발표자료/보고서 작성, 중간/최종 발표 수행
- 2019년 11월 1일 최종 본선에서 특별상 수상  
[수상관련 학과 게시물](https://sci-cube.skku.edu/sci-cube/community/news.do?mode=view&articleNo=87619&article.offset=0&articleLimit=10)  
![특별상](https://github.com/gimys/kogas_competition/blob/master/%ED%8A%B9%EB%B3%84%EC%83%81_%EC%88%98%EC%83%81.jpg)
## 4. 연구내용 요약
1. 분석용 머신은 CPU와 RAM은 제공되나 GPU가 제공되지 않는 환경으로 제공  
2. 계측된 데이터에는 이상치나 결측치가 다수 존재함  
3. 동일한 기기의 계측 값이라도 동일한 타임 프레임을 갖고 있지는 않음  
4. 공장 기기의 특성상 기계가 가동되면 계측 값도 일정 구간 내에서만 계측됨  
5. 따라서 몇초~몇분 단위의 데이터를 하루 단위로 변환하여 타임프레임, 결측값, 예측값 문제를 감소  
6. 전날의 데이터를 통해 오늘의 펌프 에너지 사용량을 예측하는 방법론 제시  
7. 운용 데이터 분석을 통해 비효율적인 펌프의 과대한 사용 현황 파악  
8. 선형회귀, 비선형회귀, 딥러닝 모델 제작  
## 5. 상세 연구 내용
- 보안 사항으로 샘플 데이터도 반출 불가하여 사용한 코드만 기록
1. [데이터 전처리 과정 notebook](https://github.com/gimys/kogas_competition/blob/master/kogas_data_merging.ipynb)
2. [데이터셋 및 모델 선정 연구 과정 notebook](https://github.com/gimys/kogas_competition/blob/master/kogas_model_proto.ipynb)
3. [모델 훈련 과정 notebook(base line)](https://github.com/gimys/kogas_competition/blob/master/(base)kogas_model_randomforest.ipynb)
