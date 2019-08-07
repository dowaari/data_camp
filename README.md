# data_camp
울산대 data date 빅데이터분석 전문가 과정(7/22~8/23)


1. 규칙
    - project 관련 위주로 올릴 것
    - 강의내용중 몰랐던 부분이나 잘이해되지 않는 부분 정리해서 올릴 것

2. **금융관련 빅데이터 분석 project 아이디어** (7/30)
    - [idea thinking 별도정리](idea_thinking.md)
    - 공공데이터 활용사례 참고사이트
        - http://www.startupidea.kr/award/
        - https://www.data.go.kr/useCase/exam/index.do
    - 금융상품별 아이디어 생각
        - 부동산, 주식, 가상화폐, 환율/원자재/금리, 신용(대출)

3. 대략적인 계획 (8/1)
    - 선행연구조사, 참고문서공부, 리뷰는 모두같이 8/3~6(회의)
    - 데이터수집: 데이터별 분담(수집,전처리,시각화,연관성분석까지) 8/6~9
    - 데이터전처리: 데이터별 분담 8/9~12(회의)
    - 데이터상관분석(통계): 1명 8/9~
    - 텍스트마이닝, 뉴스감성분석: 2명 8/9~
    - 머신러닝, 백테스팅: 1명 8/12~           
    - 웹시각화: 1명 8/9~

4. 소스코드 및 데이터 공유
    - 주소: 단톡방 공개
    - 팀원별 폴더생성, 각자 생성한 코드, 데이터를 업로드한다.

5. 프로젝트 계획 상세 (8/5)
    - 주제: 빅데이터분석을 활용한 코스피지수 예측 알림서비스
    - 목적:
        * 저금리시대에 재테크는 필수, 투자결정에 도움을 주는 정보제공서비스
        * 뉴스분석, 거시경제지표 등 다양한 지표들을 분석하여 코스피지수의 방향성을 예측하고자 한다. 
        * 선정동기 : 
            - 데이터분석을 통해 지수 예측이 가능한가? 정확도는? 변동요인은? 에 대한 의문
            - 새로운 아이디어보다는 교육과정에서 습득한 분석 기법을 제대로 응용해 보는데 중점
            - 다양한 공개데이터를 활용할수있고 참고자료가 많음.
    - 시나리오:
        * 전일까지의 데이터를 분석한다. 과거데이터의 기간은 x일(1달,1년,5년,10년)
        * 미래의 시세를 예측한다. 기간 x일(2,5,10일)에 대한 상승/하락 방향성, 변화율(%), 확률정보가 될수있다. 
        * 백테스팅: 과거 데이터를 통해 가상매매를 해보고 수익률을 확인할수있다.
        * 웹에 결과를 표 및 그래프로 시각화, 1일 카톡알림
    - 데이터수집: 수작업, 엑셀, 크롤링, OPEN API 등으로 수집하여 csv,json형태로 저장한다. 
        * 과거지수(기술적지표), 신용, 수급, 해외지수 (1)
        * 까페, 증권뉴스, 검색어트렌드 -> 네이버 (2)
        * 거시경제지표: GDP,금리,환율,수출입동향 등-> 한국은행경제통계시스템, 통계청 (2)
    - 기타:
        * 우선 코스피지수로 시작하고 의미있는 결과가 나오지 않을경우 분석대상을 다른 상품(환율,원자재)으로 변경
        * 참고내용
            - 2014년 빅데이터아카데미 우수사례집 (일일환율예측, 주가예측상관관계분석)
            - https://www.nature.com/articles/srep01684
            - 그 외 구글검색을 통한 다수의 논문들

6. 회의록 (8/6)
    - 거시경제지표 중 주가와 연관있는 지표 찾기가 쉽지않음. 
    - 애초에 생각했던 경기선행지수, 무역수지, 고용율 등 차트로 봤을때 직관적으로 연관성이 없었음. 
    - 대부분 월별 데이터임. 데이터의 개수가 부족함.
    - 거시경제지표 중 일별로 수집할수있는 거시경제지표만을 수집한다. (네이버금융->시장지표) 
        - 환율(원/달러, 엔화/달러, 위안/달러, 달러인덱스)
        - 금, 구리, 금리(국고채3년, 장단기금리차 등), 더 찾아보자.
        - 일별시점이 서로 다를때 어떻게 처리해야하나? 병합시 결측값발생, 삭제 또는 보간
    - PlanB에 대해서도 항상 생각해보자.    
    - 관련논문 더 읽어보고 정리 -> paper review.md 에 간략정리   
    - 뉴스분석 개인생각
        - 일별 뉴스기사의 갯수가 적다, 네이버증권말고도 다른 사이트에서도 수집
        - 기업명이 들어간 샘플은 제외하는 것이 좋을듯
        - 명사위주, 동사는?        

7. 모델 흐름도(생각중)
    - 데이터 수집
    - 데이터 전처리
    - EDA: feature간 상관관계, 다중회귀분석, 시계열분석(자기상관) 등 분석
    - feature engneering: 파생변수, feature 중요도 확인 -> feature 선정
    - 모델학습을 위한 dataset 구성: input feature, target
    - train / (validation) / test set 만들기
    - base model
    - Denoising + CNN Encoder + LSTM, Attention network
     
    


