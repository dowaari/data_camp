# 금융관련 빅데이터 분석 project 아이디어 정리

```
    (0) 제목
        - 목적
        - 시나리오
        - 관련 데이터
        - 역할분담 : 
        - comment:
    
    (1) 빅데이터분석을 활용한 환율예측 알림서비스
        - 목적: 1달이상의 장기적인 환율추이를 예측하여 고객이 유리한 환율조건에 환전할수있도록 한다.
        - 시나리오: 환율추이 시각화 -> 특정기간/특정조건에서 예약환전할수있는 서비스
        - 데이터: 과거환율(기술적지표), 뉴스제목(세계 정치경제 상황), 주가, 그외 경기지표
        - 역할분담: 선행연구조사 / 데이터별 수집 및 전처리 / 텍스트분석,머신러닝,벡테스팅 / 웹시각화
        - comment: 
            * 연관성 있는 데이터가 딱히 생각나지 않음. domain 지식부족
            * 뉴스제목수집 -> 텍스트 -> 단어 -> 환율에 긍정/부정인지 머신러닝
            * 참고: 2014년 빅데이터아카데미 우수사례집, 일일 환율 예측 프로젝트 p22
        
    (2) 빅데이터분석을 활용한 코스피지수예측 알림서비스
        - 목적: 
            * 텍스트마이닝과 여러 다양항 지표들을 분석하여 코스피지수의 방향성을 예측하고자 한다. 
            * 투자자들에게 투자결정판단에 도움을 주는 정보제공서비스 
            * 저금리시대 취업후 재테크는 필수, 월급으로는 10년일해도 서울에 집한채못삼. 
            * 데이터분석을 통해 예측이 가능성한지, 예측의 정확도를 높일수있는지 확인
        - 시나리오: 단기/장기 예상추세 시각화, 상승하락 확률표시 -> 1일 카톡알림 (kodex200, 인버스투자 가능)
        - 데이터: 과거지수(기술적지표),신용,수급 / 까페, 증권뉴스, 검색어트렌드 / 그외 경기지표
        - 역할분담: 선행연구조사 / 데이터별 수집 및 전처리 / 텍스트분석,머신러닝,벡테스팅 / 웹시각화       
        - comment: 
            * 환율예측과 유사하지만 조금더 다양하고 특정범위의 데이터를 구할수있음
            * 관련자료가 많아 조금더 쉬울거같음.
            * 참고 "키워드관련 지수예측", "구글트렌드 주식", "뉴스분석 주가예측" 등 구글검색해볼것.
            * https://www.nature.com/articles/srep01684
            * 참고: 2014년 빅데이터아카데미 우수사례집, 주가 예측 상관관계 분석 p16
        
    (3) 한경컨센서스의 기업보고서 알림서비스, 키워드추출 및 자동요약 메일발송
        - 목적: 
            * 개인이 주식투자시 증권사의 기업보고서 체크는 매우중요
            * 보고서의 요약정보(키워드)를 신속하게 카톡으로 알려주고 링크를 통해 보고서를 확인 
        - 시나리오: 웹에 키워드 등록 -> 10분 주기 크롤링(감시) -> 출현 -> 링크,키워드추출 -> 카톡발송
        - 데이터: 없음.
        - 역할분담: 기능별 분담, 앱개발/크롤링,알림/pdf키워드추출
        - comment: 
            * 한경컨센서스, 다트, 그 외 보고서 사이트(증권사?)
            * pdf자동 다운, pdf에서 중요키워드 추출은 어떻게?
            * 키워드에 대해 감성분석 가능, 그 외 데이터분석 또는 머신러닝 활용요소가 없음.
            * 앱과 자동화기능 연계는 어떻게?
            
    (4) 울산 아파트 시세 예측 서비스
        - 목적: 
            * 아파트 투자판단에 도움을 주는 지표를 제공한다.
            * 아파트 실거래 또는 투자목적의 상황에서 의사결정에 도움을 주는 정보제공 서비스
        - 시나리오:            
            * 분석대상은 울산의 아파트 가격으로 한정한다.
            * 특정 아파트의 최근실거래가, 현재호가, 1달후예측, 1년추세를 시각화 제공
            * 특정 아파트 주변의 교통,학군,인구변동 등 연관팩터에 대해 제공
            * 시간여유가 있으면 웹페이지 또는 앱까지
        - 데이터: 과거 실거래가 / 거시경제지표(금리) / 교통(지하철) / 학군 / 인구변동(입출) / 기업실적  
        - 역할분담: 데이터별 분담, 통합하여 머신러닝(2) 
        - comment: 
            * 구할수있는 데이터가 매우 다양? 확인필요
            * 참고예시가 많다. Dacon대회, kaggle대회, 보고서 등
            * 이미 유사서비스들이 있다.(직방,부동산지인) 차별점은? 정확도 비교 어떻게?
            * 참고: 2017년 빅데이터아카데미 우수사례집, 기계학습 방법을 활용한 신도시 아파트 가격변동 요인 분석
            * 참고 url:
                https://dacon.io/cpt4 
                https://bit.ly/2UuQvtU 
                https://www.kaggle.com/c/house-prices-advanced-regression-techniques/ 
            
            
     (5) 울산지역 살기좋은 동네찾기 서비스
        - 목적: 
            * 타지역에서 울산에 이사를 계획중인 (울산을 잘모르는) 사람이 온라인상으로 살기좋은 동네를 많이 물어봄.
            * 아이들 키우기 좋은곳, 혼자살기좋은 곳 등 정보제공의 목적
        - 시나리오: 환경/인프라/교육/치안/교통, 사용자가 선호하는 카테고리로 동네 추천
        - 데이터: 카테고리별 공공데이터 유무 확인 / 데이터통합 / 시각화
        - 역할분담: 데이터별 분담
        - comment: 머신러닝 필요없음. 클러스터링이 필요한가?
     
            
    <탈락된 아이디어> 
    
    (1) 빅데이터 분석과 머신러닝 등을 활용해 기업의 부실 징후 정보를 파악
        - 목적: 기업부실징후예측을 통해 기업평가지표, 여신심사, 주식종목분석 등에 활용할수있다.
        - 데이터: 재무상태(순이익,부채,부채비율), 대출금리, 결국 사업보고서 내용으로 한정적, 해당산업의 상황
        - comment: 구할수있는 데이터가 한정적임. domain지식이 부족함.
        
    (2) 포털사이트 뉴스 제목 분석을 통한 금리변동 예측 
        - 위의 환율추이와 유사, 금리는 변동성이 작다. 하루단위로 바뀌지않음, 데이터가 많지 않음.
   
    (3) OCR기술을 활용하여 고객 제출 서류 정보 추출하기
        - 목적: 예금가입, 대출서류, 영수증 등의 정보를 자동입력, 은행,회계 업무효율화 
        - 시나리오: 서류 스캔 -> 정해진폼에 자동입력
        - 데이터: 관련서류, 필기체 이미지
        - 역할분담: 애매함.
        - comment: 
            * OCR 관심있어서 한번 해보고싶음, 시간적여유가 없다, 역할분담은? 
            * 데이터는 어디서? 학습은? 필기체, 기술적으로 어려울수있다.
```
