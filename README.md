# Amazon E-Commerce Trends
### Objective:
Using consumer, product, and sales data, what can we determine about the effectiveness of Amazon's different "premium" labels? What do these labels actually mean to consumers?
In order to solve this, I have looked into three types of Amazon items- Prime, Sponsored, and "Amazon Choice," and compared them to the average of ALL products.

### Job Description:
The job description I chose was "Data Analyst- Inventory Deployment" at Nordstrom. The description states that analysts are to "mine complex financial data and transform it into actionable information," as well as to "apply common statistical methods, data modeling, and predictive analysis to answer strategic questions for the online business." The job primarily works with financial data, focusing on the e-commerce aspect of Nordstrom's business.
I chose to complete my project using Amazon product data, and generated sales based on the review counts of different items. This relates to the job posting because it is E-commerce sales data, and while Amazon has different offeringss than Nordstrom would (Amazon Choice and Prime), the same analysis could be run to determine the effectiveness of Nordstrom offerings if I had the right data.

## Data
In order to get the Amazon product data, I used the "Amazon Products" API from the RapidAPI website to grab the name, ASIN, price, promotions, etc. of hundreds of Amazon products. Then, I found a public dataset of consumer information from Kaggle and randomly generated 20,000 orders, with the likelihood of a product being ordered being proportional to the number of reviews on its Amazon page.
The data was stored in three tables, "product", "customer", and "customer_order". The customer_order had its own primary key, "order_id", and the table linked the two others on their respective primary keys, "asin" and "customer_id".

## Notebooks

## Future Improvements
1. I think that having real order and category data would help the project a lot. I ran out of API requests before I could get the category of each product, so I ended up assigning a category randomly to each product and not using this information very much in my analysis. Order data is usually not something that is openly available to the public, so I don't know if I could acquire it- however, this information would allow me to get REAL insight from the data that could be used to make legitimate suggestions grounded in facts.
2. If I had paid for premium API access, I could've gotten information on thousands of products, rather than hundreds, and this would also allow me to get a more complete picture of Amazon's catalogue.
