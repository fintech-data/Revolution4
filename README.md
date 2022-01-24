# Revolution4

# **#1 신용위험 분석 데이터**

<pre><code>[1]: id [NaN:0.0%] = A unique LC assigned ID for the loan listing.
[2]: member_id [NaN:0.0%] = A unique LC assigned Id for the borrower member.
[3]: loan_amnt [NaN:0.0%] = The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
[4]: funded_amnt [NaN:0.0%] = The total amount committed to that loan at that point in time.
[5]: funded_amnt_inv [NaN:0.0%] = The total amount committed by investors for that loan at that point in time.
[6]: term [NaN:0.0%] = The number of payments on the loan. Values are in months and can be either 36 or 60.
[7]: int_rate [NaN:0.0%] = Interest Rate on the loan
[8]: installment [NaN:0.0%] = The monthly payment owed by the borrower if the loan originates.
Y1 - [9]: grade [NaN:0.0%] = LC assigned loan grade 
Y2 - [10]: sub_grade [NaN:0.0%] = LC assigned loan subgrade
[11]: emp_title [NaN:5.800000000000001%] = The job title supplied by the Borrower when applying for the loan.*
[12]: emp_length [NaN:5.1%] = Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years. 
[13]: home_ownership [NaN:0.0%] = The home ownership status provided by the borrower during registration. Our values are: RENT, OWN, MORTGAGE, OTHER.
[14]: annual_inc [NaN:0.0%] = The self-reported annual income provided by the borrower during registration.
[14]:verification_status
[16]: issue_d [NaN:0.0%] = The month which the loan was funded
Y3 - [17]: loan_status [NaN:0.0%] = Current status of the loan
[18]: pymnt_plan [NaN:0.0%] = Indicates if a payment plan has been put in place for the loan
[19]: url [NaN:0.0%] = URL for the LC page with listing data.
[20]: desc [NaN:85.8%] = Loan description provided by the borrower
[21]: purpose [NaN:0.0%] = A category provided by the borrower for the loan request. 
[22]: title [NaN:0.0%] = The loan title provided by the borrower
[23]: zip_code [NaN:0.0%] = The first 3 numbers of the zip code provided by the borrower in the loan application.
[24]: addr_state [NaN:0.0%] = The state provided by the borrower in the loan application
[25]: dti [NaN:0.0%] = A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.
[26]: delinq_2yrs [NaN:0.0%] = The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years
[27]: earliest_cr_line [NaN:0.0%] = The month the borrower's earliest reported credit line was opened
[28]: inq_last_6mths [NaN:0.0%] = The number of inquiries in past 6 months (excluding auto and mortgage inquiries)
[29]: mths_since_last_delinq [NaN:51.2%] = The number of months since the borrower's last delinquency.
[30]: mths_since_last_record [NaN:84.6%] = The number of months since the last public record.
[31]: open_acc [NaN:0.0%] = The number of open credit lines in the borrower's credit file.
[32]: pub_rec [NaN:0.0%] = Number of derogatory public records
[33]: revol_bal [NaN:0.0%] = Total credit revolving balance
[34]: revol_util [NaN:0.1%] = Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
[35]: total_acc [NaN:0.0%] = The total number of credit lines currently in the borrower's credit file
[36]: initial_list_status [NaN:0.0%] = The initial listing status of the loan. Possible values are – W, F
[37]: out_prncp [NaN:0.0%] = Remaining outstanding principal for total amount funded
[38]: out_prncp_inv [NaN:0.0%] = Remaining outstanding principal for portion of total amount funded by investors
[39]: total_pymnt [NaN:0.0%] = Payments received to date for total amount funded
[40]: total_pymnt_inv [NaN:0.0%] = Payments received to date for portion of total amount funded by investors
[41]: total_rec_prncp [NaN:0.0%] = Principal received to date
[42]: total_rec_int [NaN:0.0%] = Interest received to date
[43]: total_rec_late_fee [NaN:0.0%] = Late fees received to date
[44]: recoveries [NaN:0.0%] = post charge off gross recovery
[45]: collection_recovery_fee [NaN:0.0%] = post charge off collection fee
[46]: last_pymnt_d [NaN:2.0%] = Last month payment was received
[47]: last_pymnt_amnt [NaN:0.0%] = Last total payment amount received
[48]: next_pymnt_d [NaN:28.499999999999996%] = Next scheduled payment date
[49]: last_credit_pull_d [NaN:0.0%] = The most recent month LC pulled credit for this loan
[50]: collections_12_mths_ex_med [NaN:0.0%] = Number of collections in 12 months excluding medical collections
[51]: mths_since_last_major_derog [NaN:75.0%] = Months since most recent 90-day or worse rating
[52]: policy_code [NaN:0.0%] = publicly available policy_code=1
new products not publicly available policy_code=2
[53]: application_type [NaN:0.0%] = Indicates whether the loan is an individual application or a joint application with two co-borrowers
[54]: annual_inc_joint [NaN:99.9%] = The combined self-reported annual income provided by the co-borrowers during registration
[55]: dti_joint [NaN:99.9%] = A ratio calculated using the co-borrowers' total monthly payments on the total debt obligations, excluding mortgages and the requested LC loan, divided by the co-borrowers' combined self-reported monthly income
[55]:verification_status_joint
[57]: acc_now_delinq [NaN:0.0%] = The number of accounts on which the borrower is now delinquent.
[58]: tot_coll_amt [NaN:7.9%] = Total collection amounts ever owed
[59]: tot_cur_bal [NaN:7.9%] = Total current balance of all accounts
[60]: open_acc_6m [NaN:97.6%] = Number of open trades in last 6 months
[61]: open_il_6m [NaN:97.6%] = Number of currently active installment trades
[62]: open_il_12m [NaN:97.6%] = Number of installment accounts opened in past 12 months
[63]: open_il_24m [NaN:97.6%] = Number of installment accounts opened in past 24 months
[64]: mths_since_rcnt_il [NaN:97.7%] = Months since most recent installment accounts opened
[65]: total_bal_il [NaN:97.6%] = Total current balance of all installment accounts
[66]: il_util [NaN:97.89999999999999%] = Ratio of total current balance to high credit/credit limit on all install acct
[67]: open_rv_12m [NaN:97.6%] = Number of revolving trades opened in past 12 months
[68]: open_rv_24m [NaN:97.6%] = Number of revolving trades opened in past 24 months
[69]: max_bal_bc [NaN:97.6%] = Maximum current balance owed on all revolving accounts
[70]: all_util [NaN:97.6%] = Balance to credit limit on all trades
[70]:total_rev_hi_lim
[72]: inq_fi [NaN:97.6%] = Number of personal finance inquiries
[73]: total_cu_tl [NaN:97.6%] = Number of finance trades
[74]: inq_last_12m [NaN:97.6%] = Number of credit inquiries in past 12 months
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
