# Heavy Power Nutrition Business Ad-Hoc analysis (MySQL).


### **Project Overview : “HPN”  or “Heavy Power Nutrition” USA based sports & bodybuilding products manufacturing company expanded their business to the north American , European & Latin territory ,  As a business data analyst at “HPN” task is to provide various Business ad-hoc request solution, uncovering insights , trends based on the data we have access to .



## **Business Ad-Hoc questions.

      - Generate a  customer business report with kpi  & report must be dynamic based on fiscal year and market. 
      - Identify total customers we have & active customers did business with . 
      - Write query to return top selling products by category &  a query to return products that are unsold. 
      - Query the customers who took >200 days for second order. 
      - Query country, customer wise top 5 qty returns & amount refunds .
      - Query customers having return rate > 30%  &  identify customers who bought most unique products . 
      - Query avg order value by customers  > 2000 & transactions > 100 to identify high spending customers .
      - Query profit contribution by business type & unique customers gain by fiscal year
      - Do discounts have correlation with products qty sold ?
      - Query top 10 products & least 10 products with return rate
      - Query top 3 qty per transaction of products category wise to identify fast moving products of each category.
      - Query products with most unique customers ( Top 20 ) to identify products wide distribution
      - Query region wise sales % contribution by customers.
      - Query a Product based profit report of 11 vs 12 vs 13 , create store procedure on “country” , “region” to make the report dynamic
      - Query Month over month  & Quarter over quarter sales % change .
      - Query new customer orders & repeat customer orders by orderdate .
      - Generate a finance report by year  & keep the report dynamic by country ,business type , category for multiple uses .
      - Name the products that contributes to top 20% of the profit .
      - Query Pareto (80/20)  rule of profit   for  Products & Customers . 
      - Query running total of revenue by months .
      - Query 3 month rolling avg of profit .

## Data Preparation 
![Screenshot 2024-08-19 131752](https://github.com/user-attachments/assets/bc2cd141-6b3b-4744-b089-3f3c475187db)

![Screenshot 2024-08-19 133142](https://github.com/user-attachments/assets/daa8d363-7066-4422-ac89-17bcba7ed912)
- 2 fact table is present in database , so revenue & refund view created from 2 fact tables , then populated together in kpi_view.
- Date_view is created with all kpis and dates  to do some time based calculations .
- Kpi_View = (Revenue_view+ Refund_view)  ;  Date_View = (Date+KPI_view).
## *Adhoc question 1 : Generate a  customer business report with kpi  & report must be dynamic based on fiscal year and market. 
![customer kpi code](https://github.com/user-attachments/assets/3e196d34-13b9-4580-bed0-e0e0a92e7ca4)
![customer kpi v ](https://github.com/user-attachments/assets/a8d0f8d5-e32a-43ba-b775-92c5df366aeb)

## *Adhoc question 2  :Identify total customers we have & active customers did business with ? 

![Screenshot 2024-08-19 141612](https://github.com/user-attachments/assets/f2fb05d0-73f9-40a6-9085-b81db8eea7d2) 

## **Adhoc question 3  :Write query to return top selling products by category &  a query to return products that are unsold.
![Screenshot 2024-08-19 233310](https://github.com/user-attachments/assets/5b9ebe1c-5eb6-4b28-ad0b-7ac938cef774)
## **Adhoc question 4  :Query the customers who took > avg 200 days for second order

![Screenshot 2024-08-19 233536](https://github.com/user-attachments/assets/74c4802d-1fab-4e5b-acb5-3f4309f76af0)
## **Adhoc question 5 : Query country, customer wise top 5 qty returns & amount refunds 
![Screenshot 2024-08-19 234654](https://github.com/user-attachments/assets/dca5b174-0c07-4702-92a4-ffb200a40dee)
## **Adhoc question 6 : Query customers having return rate > 30% &  identify customers who bought most unique products .
![Screenshot 2024-08-21 202348](https://github.com/user-attachments/assets/630bb72d-6e31-49e0-8e6f-c8f0f299c6df)
 ## **Adhoc question 7 : Query profit contribution by business type & unique customers gain by fiscal year.
 
![Screenshot 2024-08-21 210106](https://github.com/user-attachments/assets/c548f522-3cd8-40e0-909c-eab9ea1ada0f)

 ## **Adhoc question 8 : Query avg order value by customers  > 2000 & transactions > 100 to identify high spending customers .
 
![Screenshot 2024-08-21 210431](https://github.com/user-attachments/assets/2f77463c-cb26-49bb-b574-9b3382b5f932)
 ## **Adhoc question 9 : Do discounts have correlation with products qty sold ?![Screenshot 2024-08-21 211037](https://github.com/user-attachments/assets/d43f6980-832d-4e91-8365-feeb6969065e)

 - Protein is the most profitable product of HPN ,accounts for 92% of the profit alone , so yes discounts did induce revenue for Protein .

 ## **Adhoc question 10 : Query top 10 products & least 10 products with return rate.
 ![Screenshot 2024-08-21 212503](https://github.com/user-attachments/assets/d01df033-e993-474c-968f-1ef4f643a054)

 ## **Adhoc question 11 :  Query top 3 qty per transaction of products category wise to identify fast moving products of each category.
 ![Screenshot 2024-08-22 232117](https://github.com/user-attachments/assets/fff0faa1-7bbe-421d-83e4-3d344f99a864)
  ## **Adhoc question 12 : Query products with most unique customers ( Top 20 ) to identify products wide distribution 
  ![Screenshot 2024-08-22 232420](https://github.com/user-attachments/assets/c165adf3-acba-4dac-84af-2fc51f867e0b)
## **Adhoc question 13 : Query region wise sales % contribution by customers.
 ![Screenshot 2024-08-22 232502](https://github.com/user-attachments/assets/07af4378-624f-469b-b469-1d563374440c)
 ## **Adhoc question 14 : Query a Product based profit report of 11 vs 12 vs 13 , create store procedure on “country” , “region” to make the report dynamic
 ![Screenshot 2024-08-23 200258](https://github.com/user-attachments/assets/3213b6d3-ddbf-433a-a828-ea7342004a3b)
  ## **Adhoc question 15 : Query Month over month  & Quarter over quarter sales % change .
  ![Screenshot 2024-08-23 200455](https://github.com/user-attachments/assets/86dd6360-f3e9-4355-8a0a-fc1223fa6934)
 ## **Adhoc question 16 : Generate a finance report by year  & keep the report dynamic by country ,business type , category for multiple uses .
 ![Screenshot 2024-08-23 210044](https://github.com/user-attachments/assets/7a4b128b-a738-482d-a206-0b98d3bb3a76)
  ## **Adhoc question 17 : Name the products that contributes to top 20% of the profit .
  ![Screenshot 2024-08-23 205916](https://github.com/user-attachments/assets/b629fcfc-3d4c-4a29-b877-b6e53d0de5c1)


   ## **Adhoc question 18 :  Query Pareto (80/20)  rule of profit   for  Products & Customers .

   ![Screenshot 2024-08-24 211751](https://github.com/user-attachments/assets/8bd8ab5d-c477-4e5f-a25b-0cbeae83c27f)
   ## **Adhoc question 19 : Query new customer orders & repeat customer orders by orderdate .
   
![Screenshot 2024-08-24 214855](https://github.com/user-attachments/assets/1b61a1cc-8f06-4a35-baaa-133ac000b9e4)
   ## **Adhoc question 20 : Query Running total of revenue.
   ![Screenshot 2024-08-25 231530](https://github.com/user-attachments/assets/6afb5137-0644-487d-89d7-21dc422b3f11)



 



## Excel (Dashboard)

![Screenshot 2024-08-25 234216](https://github.com/user-attachments/assets/57640791-924e-4023-9c96-bb7e6879978b)
![Screenshot 2024-08-25 234541](https://github.com/user-attachments/assets/3bd277c7-9a60-4529-a0c3-b5b642528e3e)
![Screenshot 2024-08-25 234558](https://github.com/user-attachments/assets/03a857a5-39ad-4b8d-80f6-c00887d24bf4)
