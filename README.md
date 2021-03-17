# Home Credit Default 

一共有8个数据集，包括1个主训练集，1个测试集和6个辅助信息表。

1. application_{train|test}.csv
- 这是主表，分为两个文件，分别用于Train(有目标)和Test(没有目标)。
- 所有应用程序的静态数据。一行表示数据样本中的一笔贷款。

2. bureau.csv

- 所有客户以前由其他金融机构提供的信用报告给信用局(针对在我们的样本中有贷款的客户)。
- 对于我们的示例中的每一笔贷款，在申请日期之前，客户在信用局中拥有的信用数与行数一样多。

3. bureau_balance.csv

- 之前在信用局月贷方余额。
- 这个表有一行记录了每个月向信用局报告的每个以前的信用记录——即该表有(#loans in sample * # of relative previous credit * # of months where we have some history observable for the previous credit)行。

4. POS_CASH_balance.csv

- 以前的POS(销售点)的月余额快照和申请人在家庭信贷的现金贷款。
- 这个表有一行对于每个月的所有信贷在国内信贷的历史(消费信贷和现金贷款)相关贷款在我们的样例,即表(#loans in sample * # of relative previous credits * # of months in which we have some history observable for the previous credits)行。

5. credit_card_balance.csv

- 申请人先前持有的家庭信贷信用卡的月余额快照。
- 这表有一行对于每个月的所有信贷在国内信贷的历史(消费信贷和现金贷款)相关贷款在我们的样例,即表(#loans in sample * # of relative previous credit cards * # of months where we have some history observable for the previous credit card)的行。

6. previous_application.csv

- 在我们的样本中有贷款的客户的家庭信贷贷款的所有以前的申请。
- 在我们的数据示例中，前面每个与贷款相关的应用程序都有一行。

7. installments_payments.csv

- 还款历史为以前支付的信贷在家庭信贷相关的贷款在我们的样本。
- a)每一次付款都有一行，b)每一次错过付款都有一行。
一行等价于一个分期付款的一次付款，或者一个分期付款对应于我们的示例中与贷款相关的前一个家庭信贷的一次付款。

8. HomeCredit_columns_description.csv

- 该文件包含对各种数据文件中的列的描述。
