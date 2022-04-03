# 📊DATATON📊
## 일시 : 2022_03_08 ~ 2022_03_11
----------------------------------------------------------------
### 팀명 : 에너지 솔루션 🔋
### 팀원 : 정준아, 윤제형, 조미경
----------------------------------------------------------------
## 🌟DATATON의 목적 & 팀 각오🌟
- 목적
  - 아이펠 노드를 공부하면서 데이터 전처리의 중요성을 많이 느끼고 있다.
  - 이번 데이터톤을 통해서 대회에서 사용되는 어떤 데이터인지! 어떻게 데이터를 처리하면 좋을 지에 대해서 고민해보고 스스로 경험 해보는 시간이다.
  - 절대평가이니까 경쟁보다는 조끼리 협력해서 목표를 잘 달성해보는 것이 중요하다.
- 팀 각오
  - 주어지는 데이터는 rawdata니까 그 자체로는 의미가 없지만 가치있는 데이터로 만들어보자!
  - 부담없이! 우리가 하는 데까지 최선을 다해서 결과물을 만들어보자!!
----------------------------------------------------------------
## 📝 데이터 소개 📝
- DACON '전력사용량 예측 AI 경진대회' 에서 사용했던 데이터
  - https://dacon.io/competitions/official/235736/overview/description
- 1. train.csv
  - 60개 건물들의 2020년 6월 1일 부터 2020년 8월 24일까지의 데이터 
  - 1시간 단위로 제공
- 2. test.csv
  - 60개 건물들의 2020년 8월 25일 부터 2020년 8월 31일까지의 데이터
  - 3시간 단위로 제공(강수량의 경우 6시간 단위로 제공, 예보데이터)
- 3. sample_submission.csv
  - sample_submission 데이터 
----------------------------------------------------------------
## 📅 조 계획표 📅 
| DATE | PLAN | CODE |
| --------- | ---------------------- | ---------------------- |
| 22.03.08 (화) | 팀명, 각오, 우리의 목표 정하기 |  |
| 22.03.08 (화) | 주어진 rawdata를 살펴보면서 brainstorming해 보기 |  |
| 22.03.08 (화) | 각자 살펴 본 것을 공유하면서 데이터를 어떤 방향으로 가공할지 계획짜기 |  |
| 22.03.08 (화) | 데이터 전처리, 군집화 |  |

| DATE | PLAN | CODE |
| --------- | ---------------------- | ---------------------- |
| 22.03.09 (수)-선거일이라서 휴일 | 어제 군집화 다 못한 부분 코드짜고 고민해보기 |  |

| DATE | PLAN | CODE |
| --------- | ---------------------- | ---------------------- |
| 22.03.10 (목) | 전날 각자 짜본 코드 공유하기 |  |
| 22.03.10 (목) | 데이터 군집화 마무리 |  |
| 22.03.10 (목) | 시각화계획 수립 |  |
| 22.03.10 (목) | 인사이트 도출, 결론 정리 (피그마 이용) | [🗃️](https://www.figma.com/file/cyKya6mQ9E9eVHDjTemq2h/%EC%97%90%EB%84%88%EC%A7%80-%EC%86%94%EB%A3%A8%EC%85%98-%EC%A0%95%EB%A6%AC?node-id=0%3A1) |
| 22.03.10 (목) | 발표자료 제작 |  |

| DATE | PLAN | CODE |
| --------- | ---------------------- | ---------------------- |
| 22.03.11 (금) | 9:30까지 완성된 제출파일을( .ipynb) 깃허브에 올리고 깃허브 링크제출하기 |  |
| 22.03.11 (금) | 피그마에 우리 조 전시물 소개카드 작성 (padlet에 작성) |  |
| 22.03.11 (금) | 다른 조들 전시 작품 구경 및 Q&A 시간 |  |
| 22.03.11 (금) | 발표 |  |
----------------------------------------------------------------
## 🖥️프로젝트 내용🖥️
### 0. 우리팀의 주제
기후 변화의 각 요인과 전력 사용량의 상관관계 분석
### 1. 계획 수립
- 1-1. 당시의 데이터 배경 이해하기 - 2020년 여름의 기후적 특성, 뉴스 검색을 통해 관찰
- 1-2. 우리가 데이터에 던질 질문 설정하기
- 1-3. 가설에 따른 단계별 계획 수립
### 2. 데이터의 객관적 수치 확인
- 2-1. 기후
  - 2-1-1. 일일 강수량 데이터를 시각화
  - 2-1-2. 일일 일조량 데이터를 시각화
  - 2-1-3. 일일 기온 및 전력 사용량 추이 시각화
 - 2-2. 전력량
  - 2-2-1. 각 건물별 전력사용량 시계열로 시각화
### 3. 다양한 방법의 시각화를 통해 소비전력 패턴 관찰
  - 3-1. 각 건물의 주간, 일간 전력사용량 시각화
### 4. 데이터 군집화
- 4-1. K-mean 클러스터링을 통해 군집화 시도
- 4-2. 군집화를 이룬 객체를 히트맵으로 시각화
### 5. 군집화된 소비전력패턴과 각 기후 요소간 상관관계 분석
- 5-1. 주간 소비전력과 주간 기후변화의 상관관계 관찰
### 6. 피어슨 상관계수를 사용하여 전체 군집과 기후 요소의 상관계수 측정
- 6-1. 개념정리
- 6-2. 기온과 전력량의 상관계수
- 6-3. 습도와 전력량의 상관계수
- 6-4. 일조량과 전력량의 상관계수
- 6-5. 바람과 전력량의 상관계수
- 6-6. 전체 데이터 분포
### 7. 불쾌지수에 따른 전력사용량 측정
- 온도가 전력사용량에 가장 큰 상관관계를 지니는 요인이라는 관측에 따라 불쾌지수를 측정하고 기온상승과 전력사용량의 상관관계를 관찰하기 위해 측정해 보았다.
### 8. 결론
- 지금까지 2020년 6월 1일부터 8월 00일까지 60개의 건물에서 소요된 전력량과 기후 데이터를 시각화하여 각 건물의 전력 소요량 패턴과 기후변화를 정량적으로 관측하였고 전력 소요량과 각 기후변화 요소간 상관관계가 존재하는지, 만약 존재한다면 정량적 수치로 얼마나 관계가 있을지 측정하여 보았습니다. 지금까지 과정을 통해 관찰된 결과를 제시하고자 합니다. 

   1. 전력사용량은 건물 용도와 전력 수요에 따라 비슷한 전력 소요 흐름이 나타나는 경향을 보이나, 고유한 전력 흐름을 가지는 건물도 존재한다. 
   2. 전력사용량은 여름철 기후변화 중 기온의 변화에 따른 상관관계를 가지는 경향을 보인다. 
   3. 그러나 기온 변화는 일조량의 변화와 직접적인 상관관계를 가지지 않는 경우도 관찰된다.
   4. 따라서 전력사용량을 분석하고 예측하려면 기온 변화 요인으로 일조량 뿐만 아니라 온실가스 축적, 실외기 사용으로 인한 도시 기온 상승 등을 고려하고 다양한 관점에서 접근하여 전력사용량을 분석함이 권장되며 추가적인 데이터와 조사가 필요하다.
### (번외) 비전기 냉방설비운용 여부에 따른 전력량 변화
- + 태양광 설치 여부에 따른 일조량과 전력사용량 비교
- ++ 태양광 설치 여부에 따른 기온과 전력사용량 비교
- +++ 비전기냉방설비 운영 여부에 따른 기온과 전력사용량 비교

----------------------------------------------------------------
## 🙂느낀점🙂
-배운점
  - 다양하게 데이터들을 가공시켜보고 시각화까지 시켜보면서 많이 배울 수 있었던 것 같다. 
  - 데이터에 대한 이해와 그 데이터를 관찰하고 들여다보는 시간을 좀 더 가져야한다는 생각이 들었다. 또한 이때까지 노드나 공부를 혼자서 했지만 이번에 조에서 사람들과 하면서 협력해서 결과물을 만들어내는 좋은 시간이었다.
  - 조끼리 비대면으로 해야해서 코드를 공유하거나 다같이 보면서 생각을 정리하는데 한계가 있다고 생각을 했다. 하지만, 서로서로 배려하면서 자신있는 부분들을 나눠서 코드를 짜보고 정리를 하니까 자신이 부족했던 부분을 서로 채워준 것 같고 내가 하지 못한 부분을 하신 것을 보고 많이 배울 수 있었던 것 같다. 
  - DACON 에 있는 다양한 코드를 보게 되었는데, 똑같은 데이터를 가지고 코드가 짜여져있어 좋은 코드를 참고해보기도 좋았고 같은 표현을 해도 다양한 코드가 나오니까 흥미롭고 많이 배웠던 것 같다.

-아쉬운점
  - 데이터를 보면서 도전해보고, 다양하게 시도를 해보고 싶었는데 시각화를 시키고 데이터를 가공하는데 생각보다 잘 되지 않았다. 그래서 다양한 도전과 아이디어들을 다 표현하지 못 한것 같아서 너무 아쉬운 것 같다. 또한 코드를 전부 짜지는 못하겠지만, 다른 사람의 코드를 보고 바꿔보고 저희 코드로 변경도 시켜보려고 했지만 에러가 너무 뜨고 생각보다 잘 되지 않아서 아직까지는 코드에 대한 이해도나 직접 시각화를 시키는 역량이 부족했던 것 같다.
  - 처음에 재밌게 여러가지 다양한 가설들을 세워보았는데 시간적으로도 너무 부족해서 아쉬웠다. 온도를 높이는 요인이 일조량이 아니라는 것을 알게 되었는데 뒤늦게 알게 되어 불쾌지수를 구해보거나 태양광 설치 여부 같은 시도를 더 못해봐서 아쉽다.
  - 처음에 5가지 주제 중에서 전력사용량이 데이터 양이 작기도 하고 한글로 되어있어서 이 정도는 한 번 해볼 수 있겠다~ 싶어서 선택을 했다. 하지만 데이터가 양이 작으니 분석을 하는데 어려움이 컸던 것 같다. 
