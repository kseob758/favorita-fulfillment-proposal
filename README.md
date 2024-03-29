# favorita-fulfillment-proposal
<p>
  <img src="https://github.com/kseob758/favorita-fulfillment-proposal/assets/125840318/8c486125-2d8b-41f2-9ceb-f170799172b4" width="700" height="350">
</p>

### 타깃 및 상황
- 에콰도르의 유통 전문 대기업 FAVORITA 그룹
- 고객의 구매 패턴이 온라인으로 전환 중인 시장 환경에 따라 직면할 위기에 대비하며 "에콰도르 최대의 유통업계" 타이틀 유지를 목표로 한다.
- 타깃(FAVORITA 전략기획팀장)은 온라인 물류 시스템 최적화를 위한 풀필먼트 시스템을 도입하기 위해 데이터 분석 팀에게 분석을 의뢰했다.
- 데이터 분석을 통해 위험성을 최소화하는 **시범 사업 세부 전략을 수립**하여 타깃에게 제공한다.
<br>

### 데이터 설명
- 에콰도르 FAVORITA의 매장 1~54번에 대한 거래 데이터
- date, store_nbr, family(제품군), sales, onpromotion(프로모션 중인 제품 개수), dcoilwtico(유가), city, state, type, cluster 등의 데이터 존재
<br>

### 데이터 분석 과정
- 왜 Quito인가? (시범 사업 시행 지역을 Quito로 결정한 이유)
  <p align="left">
  <img src="https://github.com/kseob758/favorita-fulfillment-proposal/assets/125840318/ce63eb7e-c057-489c-937e-fbfebf7866bb" width="600">
  </p>
  - Quito는 에콰도르의 수도
  - 인구수 최대 도시인 Guayaquil보다 더 많은 매장 밀집 → 일부 매장 개편 시 비교적 낮은 리스크
  - 도심지역이므로 온라인 판매 채널 확대 시 큰 효과 기대

- 3단계의 필터링 과정을 통해 전환할 매장 선정
<p align="left">
  <img src="https://github.com/kseob758/favorita-fulfillment-proposal/assets/125840318/d0f9ab23-0552-4138-b721-c882e6f31775" width="400">
</p>
    
- 추가 : 시계열 모델 Neural prophet을 활용한 재고 변동 비율 확인, 재고 관리에 도움
<p align="left">
  <img src="https://github.com/kseob758/favorita-fulfillment-proposal/assets/125840318/26bfdec1-e37c-4bcb-82f9-5d2aa7d22efd" width="600">
</p>
<br>

### 결론
Dark Store와 Semi-Dark Store 전환에 가장 적합한 매장 각각 선정
- Sales 규모, Sales 증가율, Transaction이 모두 최하위인 **10번 매장을 Dark Store로** 전환
- Sales 규모와 Transaction이 최상위지만 Sales 증가율은 규모에 비해 저조한 **44번 매장을 Semi-Dark Store로** 전환
<br>

### 기대 전망
- 도심형 물류센터 도입으로 퀵커머스 경쟁 관점에서 유리
- 기존의 매장을 전환하는 것이므로 새로운 부동산 매입에 대한 부담 없음
- 온라인 전용 공간 확보를 통해 재고 정확도 향상, 식재료 품목 관리 용이
