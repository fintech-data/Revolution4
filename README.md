# Revolution4

## **#1 신용위험 분석 데이터**

<pre><code> 컬럼명 생략
</code></pre>



#### **데이터 불러오기**
<pre><code>loan = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution4/main/data/loan.csv')
</code></pre>

## **#2 계좌 정보 데이터**

<pre><code>- CLIENTNUM: <i>int</i>,  고객번호
- Attrition_Flag: <i>str</i>, 현재 상태
- Customer_Age: <i>int</i>,  고객 연령
- Gender: <i>str</i>, 결혼여부
- Dependent_count: <i>int</i>,  부양가족수
- Education_Level: <i>str</i>, 교육수준
- Marital_Status: <i>str</i>, 결혼 상태
- Income_Category: <i>str</i>, 연간 소득액 기준
- Card_Category: <i>str</i>, 카드 등급
- Months_on_book: <i>int</i>, 은행거래 기간 (월 단위)
- Total_Relationship_Count: <i>int</i>,  총 보유계좌
- Months_Inactive_12_mon: <i>int</i>,  거래내역 없는 거래월 수
- Contacts_Count_12_mon: <i>float</i>, 거래기간 있는 거래월 수
- Credit_Limit: <i>int</i>,  신용한도
- Total_Revolving_Bal: <i>int</i>,  신용카드에서 결제해야 할 평균 금액
- Avg_Open_To_Buy: <i>float</i>, 추가 결제를 위한 신용한도 승인액
- Total_Amt_Chng_Q4_Q1: <i>float</i>, 1분기 대비 4분기 카드 거래금액 비율
- Total_Trans_Amt: <i>int</i>, 12개월 동안의 총 거래금액
- Total_Trans_Ct: <i>int</i>, 12개월 동안의 총 거래건수
- Total_Ct_Chng_Q4_Q1: <i>float</i>,	1분기 대비 4분기 거래건수 비율
- Avg_Utilization_Ratio : <i>float</i>, 평균 카드 이용률
</code></pre>

#### **데이터 불러오기**
<pre><code>bank_customers = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution/main/data/Bank_customers_data.csv')
</code></pre>

## #3. 다이렉트 마케팅 데이터

<pre><code>- Age: <i>int</i>, 나이
- Gender: <i>str</i>, 성별
- OwnHome: <i>str</i>, 주택보유여부(자가/임대)
- Married: <i>str</i>, 결혼여부
- Location: <i>str</i>, 집에서 마트까지 거리 (Far : 도보 30분 이상/close : 도보 30분 이내)
- Salary: <i>int</i> 연봉
- Children: <i>int</i>, 자녀수
- History: <i>str</i>, 회원가입연수 (5년 이상 : high, 2~5년 : Middle, 1년 이내 : Low)
- Mailing: <i>int</i>, 쇼핑몰 뉴스레터 발송횟수
- **AmountSpent: <i>int</i>, 연간 쇼핑몰 이용액**
</code></pre>

#### **데이터 불러오기**
<pre><code>direct_marketimg = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution/main/data/DirectMarketing.csv')
</code></pre>

## **#4 건강보험 및 신용 데이터**

<pre><code>- Agency: <i>str</i>, 보험 판매점
- Agency Type: <i>str</i>, 판매점 형태
- Distribution Channel: <i>str</i>, 판매 채널
- Product Name : <i>str</i>,  판매 상품 종류
- Duration: <i>str</i>, 보험기간
- Destination: <i>str</i>,  여행국가
- Net Sales: <i>int</i>, 순마진
- Commision (in value): <i>float</i>, 수수료
- Gender: <i>str</i>, 성별
- Age: <i>int</i>, 나이
- Claim: <i>str</i>, 보험료 청구
</code></pre>

#### **데이터 불러오기**
<pre><code>travel_insurance = pd.read_csv("https://raw.githubusercontent.com/fintech-data/Revolution/main/data/travel%20insurance.csv")
</code></pre>
