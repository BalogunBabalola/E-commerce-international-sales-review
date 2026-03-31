### E-Commerce sales review: Uncovering customer purchasing trends and sales pattern.

## Problem Statement:
An online retail company based in the UK lacks visibility into which products drive the most volume and revenue, when customers are most active, and who its highest-value and most loyal customers are. Without this information, decisions around inventory management, marketing timing and customer retention are made without data backing.  Using purchases data from the business, this analysis identifies the top-performing products by quantity and revenue, uncovers peak purchasing periods by hour and month and profiles the most valuable and loyal customers.

## Methodology:
The dataset consists of 541,909 records upon arrival. A total of 10,624 negative quantities were found which consisted of returned goods and cancelled orders. 25% (135,080) of the customer IDs were blank representing guest checkouts of the site.Data cleaning and initial exploration was done in Python and exported to a CSV file. For simplicity and speed, United Kingdom transactions were excluded to focus on international purchasing behaviour and returns which were identified as InvoiceNo starting with “C” were also excluded bringing the needed records to approximately 45,000. Total sales, Salesday and Saleshour were created from the Invoicedate to be used for further analysis. 

! [The dashboard] (<img width="1338" height="450" alt="final_dashboard" src="https://github.com/user-attachments/assets/aa7de7a8-8fbc-417d-8f54-fe340bc526db" />)

## Key findings:
* Between 2010 & 2011, total items sold was summed to **924,078** with the bestselling products being Rabbit Night Light constituting **28.20% (15,486)** of products sold alongside **Mini Paint Set Vintage** at **22.80% (12,601)** and **Pack of 72 Retrospot Cake Cases** selling **11,433** quantities. **Regency Cakestand 3-tier** pulling in **$32,211.45**, **Rabbit Night Light** brought in **$28,877** and **Round Snack Boxes set of 4 Woodland** at **$18,504.55(9.66%)** were top products revenue-wise. Other top products included **Spaceboy Lunch box** sold an amount of **$14,470** and **Dollygirl Lunch box** with **$12,595**

* The company’s total revenue for the period is **$1,575,267**. The company sells more on **Thursday**, **Wednesday** and **Tuesday** with the total of **$413,921.4**, **$310.338.3** and **$293,045.7** respectively for that period. Sales peak between the **10:00am** and **2:00pm** before a steady decline starts from **4:00pm**.

* A total of **419** unique customers reflects international customers excluding the UK customer base patronised the business for that period with their **Average Order Value (AOV)** being **$824.90**. Top 3 repeat customers by invoice are **customer 14911** who bought **51%** of the inventory followed by **customer 14646** who bought **18%** and **customer 14156** who bought **14%** with the rest of inventory spread across with the remaining customers while **guests’ checkouts** were estimated at **13%**. On the revenue side, **customer 14646** generated **$280,206** in revenue, **customer 14911** generated **$143,825** followed by **customer 12415** who generated **$124,914** while **guest checkouts** totalled **$38,446** in revenue.

## Recommendations:
 •	**Concentrate inventory investment on volume leaders:** Rabbit Night Light, Mini Paint Set Vintage and Retrospot Cake Cases collectively account for over 70% of units sold. Ensure these lines maintain sufficient stock levels at all times. A stockout on any of these three directly impacts the majority of sales volume.

 •	**Time marketing campaigns between 10am and 12pm on Thursdays:** Sales peak between 10am–2pm with Thursday being the highest revenue day at $413,921. Promotional emails, discount campaigns and new product launches should be scheduled to land before 10am on Thursdays to intercept customers at their highest purchase intent window.

•	**Build a VIP retention programme around the top 5 customers:** Five customers led by 14646 ($280K) and 14911 ($143K) represents the outliers of total revenue. The business is dangerously exposed if any of these accounts churn. A dedicated retention strategy (exclusive pricing, early access, account management) should be implemented immediately for this cohort.

•	**Convert guest checkouts into identified customers:** $38,446 in revenue is completely unattributable to identified customers. These are buyers the business cannot remarket to, cannot track for retention, and cannot analyse for behaviour. Introducing a post-purchase account creation incentive (discount on next order) would convert a portion of this anonymous revenue into trackable customer relationships.

## Limitations:
•	Analysis covers international transactions only since UK is excluded

•	Guest checkouts (25% of CustomerIDs) cannot be tracked behaviourally

•	Dataset covers 2010–2011 only and may not reflect current trading patterns

•	Cancelled orders were excluded from all calculations

•	Manual and Postage were excluded from descriptions
