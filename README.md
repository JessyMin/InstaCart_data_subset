요약 InstaCart 데이터로 SQL 실습 시, Import 시간을 단축할 목적으로 데이터를 샘플링함


## Objective
직장인이나 학생이 SQL을 독학하고자 할 때, 실무에서 SQL서버에 접속 가능한 환경이 아니라면 적절한 실습용 데이터셋이 필요하다.
이 reporitory는 본인의 필요에 의해 Instacart 데이터를 SQL에 옮겨넣기 위해 수행한 과정을 기록한 것이다. </br></br>


## Data Overview
Kaggle에 올라온 InstaCart 데이터는 아래 링크에서 다운받을 수 있다. </br>
<a href="https://www.kaggle.com/c/instacart-market-basket-analysis/data">
Kaggle : Instacart Market Basket Analysis </a></br>

이 데이터에 대한 상세한 설명은 아래 Instacart 공식 블로그 글에서 확인할 수 있다. </br>
<a href="https://tech.instacart.com/3-million-instacart-orders-open-sourced-d40d29ead6f2"> 
3 Million Instacart Orders, Open Sourced </a></br>

데이터셋은 총 6개의 csv 파일로 구성되어 있다. 아래 리스트 중에서 order.csv와(약 342만건) product_order__*.csv(약 3382만건)의 크기를 축소하였다.

<li>order.csv</li>
<li>order_products__prior.csv</li>
<li>order_products__train.csv</li>
<li>products.csv</li>
<li>aisles.csv</li>
<li>departments.csv</li>
</br>
</br>


## getmax.R
mySQL에서 테이블 스키마를 작성하기 위해, 각 column별로 max값을 파악하기 위한 함수이다.
(작성중)


## subset.R

mySQL에서 Table Data Import Wizard로 데이터를 가져오면 시간이 많이 소요된다. 
이에 order.csv와 order_products__#.csv의 크기를 샘플링을 통해 축소하였다. (작성중)

