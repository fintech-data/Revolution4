# Revolution4

# **#1 신용위험 분석 데이터**

<pre><code>- id = A unique LC assigned ID for the loan listing.
- member_id = A unique LC assigned Id for the borrower member.
- loan_amnt = The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
- funded_amnt = The total amount committed to that loan at that point in time.
- funded_amnt_inv = The total amount committed by investors for that loan at that point in time.
- term = The number of payments on the loan. Values are in months and can be either 36 or 60.
- int_rate = Interest Rate on the loan
- installment = The monthly payment owed by the borrower if the loan originates.
- grade = LC assigned loan grade
- sub_grade = LC assigned loan subgrade
- emp_title = The job title supplied by the Borrower when applying for the loan.*
- emp_length = Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years. 
- home_ownership = The home ownership status provided by the borrower during registration. Our values are: RENT, OWN, MORTGAGE, OTHER.
- annual_inc = The self-reported annual income provided by the borrower during registration.
- verification_status
- issue_d = The month which the loan was funded
- loan_status = Current status of the loan
- pymnt_plan = Indicates if a payment plan has been put in place for the loan
- url = URL for the LC page with listing data.
- desc = Loan description provided by the borrower
- purpose = A category provided by the borrower for the loan request. 
- title = The loan title provided by the borrower
- zip_code = The first 3 numbers of the zip code provided by the borrower in the loan application.
- addr_state = The state provided by the borrower in the loan application
- dti = A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.
- delinq_2yrs = The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years
- earliest_cr_line = The month the borrower's earliest reported credit line was opened
- inq_last_6mths = The number of inquiries in past 6 months (excluding auto and mortgage inquiries)
- mths_since_last_delinq = The number of months since the borrower's last delinquency.
- mths_since_last_record = The number of months since the last public record.
- open_acc = The number of open credit lines in the borrower's credit file.
- pub_rec = Number of derogatory public records
- revol_bal = Total credit revolving balance
- revol_util = Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
- total_acc = The total number of credit lines currently in the borrower's credit file
- initial_list_status = The initial listing status of the loan. Possible values are – W, F
- out_prncp = Remaining outstanding principal for total amount funded
- out_prncp_inv = Remaining outstanding principal for portion of total amount funded by investors
- total_pymnt = Payments received to date for total amount funded
- total_pymnt_inv = Payments received to date for portion of total amount funded by investors
- total_rec_prncp = Principal received to date
- total_rec_int = Interest received to date
- total_rec_late_fee = Late fees received to date
- recoveries = post charge off gross recovery
- collection_recovery_fee = post charge off collection fee
- last_pymnt_d = Last month payment was received
- last_pymnt_amnt = Last total payment amount received
- next_pymnt_d = Next scheduled payment date
- last_credit_pull_d = The most recent month LC pulled credit for this loan
- collections_12_mths_ex_med = Number of collections in 12 months excluding medical collections
- mths_since_last_major_derog = Months since most recent 90-day or worse rating
- policy_code = publicly available policy_code=1
new products not publicly available policy_code=2
- application_type = Indicates whether the loan is an individual application or a joint application with two co-borrowers
- annual_inc_joint = The combined self-reported annual income provided by the co-borrowers during registration
- dti_joint = A ratio calculated using the co-borrowers' total monthly payments on the total debt obligations, excluding mortgages and the requested LC loan, divided by the co-borrowers' combined self-reported monthly income
- verification_status_joint
- acc_now_delinq = The number of accounts on which the borrower is now delinquent.
- tot_coll_amt = Total collection amounts ever owed
- tot_cur_bal = Total current balance of all accounts
- open_acc_6m = Number of open trades in last 6 months
- open_il_6m = Number of currently active installment trades
- open_il_12m = Number of installment accounts opened in past 12 months
- open_il_24m = Number of installment accounts opened in past 24 months
- mths_since_rcnt_il = Months since most recent installment accounts opened
- total_bal_il = Total current balance of all installment accounts
- il_util = Ratio of total current balance to high credit/credit limit on all install acct
- open_rv_12m = Number of revolving trades opened in past 12 months
- open_rv_24m = Number of revolving trades opened in past 24 months
- max_bal_bc = Maximum current balance owed on all revolving accounts
- all_util = Balance to credit limit on all trades
- total_rev_hi_lim
- inq_fi = Number of personal finance inquiries
- total_cu_tl = Number of finance trades
- inq_last_12m = Number of credit inquiries in past 12 months
</code></pre>


#### **데이터 불러오기**
<pre><code>loan = pd.read_csv('https://media.githubusercontent.com/media/fintech-data/Revolution4/main/loan.csv')
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
