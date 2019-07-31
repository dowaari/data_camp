# data_camp
울산대 data date 빅데이터분석 전문가 과정(7/22~8/23)


1. 규칙
    - project 관련 위주로 올릴 것
    - 강의내용중 몰랐던 부분이나 잘이해되지 않는 부분 정리해서 올릴 것

2. **금융관련 빅데이터 분석 project 아이디어**

```
    (0) 제목
        - 목적
        - 시나리오
        - 관련 데이터
        - 역할분담 : 데이터별, 기능별
        - comment
    
    (1) 빅데이터 분석과 머신러닝 등을 활용해 기업의 부실 징후 정보를 파악
        - 목적: 기업부실징후예측을 통해 기업평가지표, 여신심사, 주식종목분석 등에 활용할수있다.
        - 데이터: 재무상태(순이익,부채,부채비율), 대출금리, 결국 사업보고서 내용으로 한정적, 해당산업의 상황
        - comment: 구할수있는 데이터가 한정적임. domain지식이 부족함.
       
    (2) 환율추이를 분석하여 고객에게 환전서비스 제공 
        - 환율추이를 알수있는 데이터는? 과거환율, 세계정치상황(뉴스) 너무 어렵다.
        - 포털사이트 뉴스제목분석 -> 텍스트 -> 환율에 긍정/부정 판단
        - 앱 또는 웹서비스 시각화
        - 특정기간 추천: 특정기간/특정조건에서 분할환전(예약환전)
        - comment: 
        
    (3) 포털사이트 뉴스 제목 분석을 통한 금리변동 예측 
        - 방법론에서 2번과 유사
        
    (4) OCR기술을 활용하여 고객 제출 서류 정보 추출하기
        - 목적: 예금가입, 대출서류, 영수증 등의 정보를 자동입력, 은행,회계 업무효율화 
        - 시나리오: 서류 스캔 -> 정해진폼에 자동입력
        - 데이터: 
        - 역할분담:
        - comment: 
            * OCR 관심있어서 한번 해보고싶음, 시간적여유가 없다, 역할분담은? 
            * 데이터는 어디서? 학습은? 필기체
            * 기술적으로 어려울수있다.
        
    (5) 한경컨센서스에서 특정기업 관련 보고서 출현시 알림기능, 키워드추출 및 자동요약 메일발송
        - 목적: 개인이 주식투자시 증권사의 기업보고서 체크는 매우중요, 자동화를 통해 신속하고 편리하게 보고서를 확인 
        - 시나리오: 웹/앱에 키워드 등록 -> 10분 주기 크롤링(감시) -> 출현 -> 링크,키워드추출 -> 카톡발송
        - 데이터: 없음.
        - 역할분담: 기능별 분담, 앱개발/크롤링,알림/pdf키워드추출
        - comment: 
            * 한경컨센서스와 다트 동시에
            * pdf자동다운-> 분석 -> 중요키워드 추출 어떻게?
            * 데이터분석 또는 머신러닝 이용 요소가 없다.
            * 앱과 자동화기능 연계는 어떻게?
        
    (6) 부동산 아파트 가격 예측
        - 목적: 아파트 투자판단에 도움을 주는 지표를 제공한다.
                아파트 실거래 또는 투자목적의 상황에서 의사결정에 도움을 주는 정보제공 서비스
        - 시나리오:            
            * 분석대상은 울산의 아파트 가격으로 한정한다.
            * 특정 아파트의 최근실거래가, 현재호가, 1달후예측, 1년추세를 시각화 제공
            * 특정 아파트 주변의 교통,학군,인구변동 등 연관팩터에 대해 제공
            * 시간여유가 있으면 웹페이지 또는 앱까지
        - 데이터: 과거 실거래가 / 거시경제지표(금리) / 교통(지하철) / 학군 / 인구변동(입출) / 기업실적  
        - 역할분담: 구할수있는 데이터별로 수집(5) -> 전처리,시각화,연관성분석(5) -> 통합하여 머신러닝(2) ->
        - comment: 
            * 구할수있는 데이터가 매우 다양함.
            * 참고예시가 많다. Dacon대회, kaggle대회, 보고서 등
            * EDA 다양한 지표들을 전처리하고 분석하는데 시간이 오래걸림, 난이도가 높아질수있음.
            * 이미 유사서비스들이 있다.(직방) 차별점은? 정확도 비교 어떻게?
            * 먼가 새로운것을 만든다기보다는 데이터분석을 실습해보기 위한 용도
            
        
    (7) 주식 또는 가상화폐 가격 예측
        - 캐글 대회 확인
```

3. 공공데이터 활용사례 참고사이트
    - https://www.data.go.kr/useCase/exam/index.do

4. 참고
    - 깃헙 파일을 코랩에서 보기: https://colab.research.google.com -> 깃헙주소붙여넣기

5. 아이디어 정리(7/30)
금융상품별로 생각해보기
    - 부동산
    - 주식
    - 가상화폐
    - 환율, 금리

    
    
