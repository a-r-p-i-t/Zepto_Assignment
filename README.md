# **eCommerce Transactions Data Science Assignment**  

## Table of Contents

- [Objective](#objective)
- [Installation](#dataset-description)
- [Data Description](#data-description)
- [Tasks Completed](#tasks-completed)
- [Results and Key Takeaways](#results-and-key-takeaways)
- [Customer Results Report](#customer-results-report)
- [Important Visualisations](#important-visualisations)

## **Overview**  
This project analyzes an **eCommerce Transactions dataset** to extract insights, build a lookalike model for customer similarity, and perform customer segmentation using clustering. The analysis helps in understanding customer behavior, product performance, and transaction trends, which can aid business decision-making.  


## **Dataset Description**  
The dataset consists of three files:  

1. **Customers.csv** – Contains customer details such as ID, name, region, and signup date.  
2. **Products.csv** – Contains product details including ID, name, category, and price.  
3. **Transactions.csv** – Records transactions with details such as transaction ID, customer ID, product ID, date, quantity, and total value.  

---

## **Tasks Completed**  

### **1️⃣ Exploratory Data Analysis (EDA) & Business Insights**  
- Conducted **data cleaning** (handling missing values, checking duplicates).  
- Performed **statistical analysis** on customers, products, and transactions.  
- Created **visualizations** for revenue trends, customer spending behavior, product popularity, and signup trends.  
- Extracted **5 key business insights** from the analysis.  

**Deliverables:**  
📂 `Arpit_Mohanty_EDA.ipynb` (EDA Code)  
📄 `Arpit_Mohanty_EDA.pdf` (Business Insights Report)  

---

### **2️⃣ Lookalike Model**  
- Built a **customer similarity model** using purchase history and customer attributes.  
- Recommended **3 similar customers** for each of the first 20 customers (`C0001 - C0020`).  
- Assigned **similarity scores** based on transaction patterns and product preferences.  

**Deliverables:**  
📂 `Arpit_Mohanty_Lookalike.ipynb` (Model Code)  
📄 `Arpit_Mohanty_Lookalike.csv` (Top 3 Lookalike Customers for Each User)  

---

### **3️⃣ Customer Segmentation (Clustering)**  
- Used **TotalSpend** and **TotalQuantity** for segmentation.  
- Applied the **Elbow Method** to determine the optimal number of clusters (`k=2`).  
- Visualized customer segments in a **3D plot** for better interpretation.  
- Evaluated cluster performance using:  
  - **Davies-Bouldin Index**: `0.63`  
  - **Silhouette Score**: `0.547`  
  - **Calinski-Harabasz Index**: `333.18`  
  - **Adjusted Rand Index (ARI)**: `1.0`  
  - **Mutual Information (MI)**: `1.0`  

**Deliverables:**  
📂 `Arpit_Mohanty_Clustering.ipynb` (Clustering Code)
📄 `Arpit_Mohanty_Clustering.pdf` (Segmentation Report)  


---

**Results and Key Takeaways**
### Business Insights Derived from Exploratory Data Analysis (EDA)

1. Signup Trends Over the Years
Customer signup trends indicate a rise in signups in the year 2024. This could be linked to promotional campaigns, new product launches, or changes in the company’s customer acquisition strategies. Monitoring these trends can help refine future customer outreach programs. There has been a decline in signups in the year 2023 as compared to 2022, but 2024 has seen a good increase in signup count.
2. Customer Distribution Over Region
The majority of the customers of the company are from South America, followed by Europe. The company has approximately a similar number of customers from Asia & North America.
3. Product Category Popularity
The Electronics and Books categories dominate sales, with products like smartwatches and biographies being frequently purchased. Home decor and clothing products have lower sales volume, indicating a possible need for better promotions or revised product offerings in these segments.
4. Revenue Trends Over Time
Total revenue trends show seasonal fluctuations, with spikes in sales occurring at specific periods. Peak sales occur in the months of July to mid-September. October to November shows a rapid decrease in the sales for the company.
5. Top 10 Most Purchased Products.
The top 10 products which are most sold are ActiveWear Smartwatch, SoundWaves Headphones, BookWorld Biography, ActiveWear Rug, SoundWave Cookbook, HomeSense Desk Lamp, ActiveWear Jacket, TextPro Textbook, TechPro T-Shirt, ActiveWear Textbook
6. Customer Spending Patterns
The analysis of customer spending per unit nearly follows a normal distribution, with most of the sales in between Rs 200 and Rs 350. This indicates an user spends nearly 200-350 rupees for buying a product.


### Customer Results Report
Overview
In this clustering analysis, we segmented customers based on their total spending (TotalSpend) and total quantity purchased (TotalQuantity). Other features were evaluated but did not significantly contribute to meaningful segmentation.
Methodology
Feature Selection: TotalSpend and TotalQuantity were chosen as the primary clustering parameters.
Elbow Method: The optimal number of clusters was determined using the Elbow Method, which identified k = 2 as the best choice.
Cluster Visualization: A 3D plot of customer clusters was created to assess the separation and accuracy of clustering visually.
Clustering Metrics
To evaluate the clustering performance, several key metrics were computed:
Davies-Bouldin Index: 0.63 (Lower values indicate better-defined clusters)
Silhouette Score: 0.547 (Closer to 1 indicates well-separated clusters)
Calinski-Harabasz Index: 333.18 (Higher values indicate better clustering)
Adjusted Rand Index (ARI): 1.0 (Perfect agreement with ground truth)
Mutual Information (MI): 1.0 (Indicates high information similarity)
Conclusion
The clustering results demonstrate well-separated and well-defined clusters, with k=2 being the optimal choice. The high Silhouette Score and Calinski-Harabasz Index indicate strong cluster separation, while the low Davies-Bouldin Index confirms cluster compactness. The ARI and MI values of 1.0 suggest that the clustering model aligns perfectly with an ideal classification.
Overall, this segmentation provides valuable insights into customer purchasing behavior and can be used for targeted marketing and personalized customer engagement.


**Important Visualisations**

<img src="https://github.com/user-attachments/assets/7b2b8462-5ee0-4c04-a940-3f2c15c9a119" alt="Screenshot 2025-02-02 231338" width="700">
<br><br><br><br>
<img src="https://github.com/user-attachments/assets/e1460ece-f279-4b8f-a882-033a5be4a473" alt="Screenshot 2025-02-02 231332" width="700">
<br><br><br><br>
<img src="https://github.com/user-attachments/assets/669fd3c2-78ee-453e-a184-437325ac0424" alt="Screenshot 2025-02-02 231323" width="700">
<br><br><br><br>
<img src="https://github.com/user-attachments/assets/99bcf14e-b748-4e5c-b513-03bb5faaa40d" alt="Screenshot 2025-02-02 231257" width="700">
<br><br><br><br>
<img src="https://github.com/user-attachments/assets/0f6b6e55-c34a-477a-8b10-37c12272178d" alt="Screenshot 2025-02-02 231312" width="700">
<br><br><br><br>
<img src="https://github.com/user-attachments/assets/13012afe-b0db-4437-81bf-83d17c6d40bc" alt="2025-02-02 231250" width="700">
<br><br><br><br>
<img src="https://github.com/user-attachments/assets/61804d44-efea-43f8-9e82-5b8db1ba01ca" alt="2025-02-02 231244" width="700">
<br><br><br><br>
<img src="https://github.com/user-attachments/assets/72e15683-1ba7-43a6-8b31-fe638ee78984" alt="2025-02-02 231236" width="700">
<br><br><br><br>









\







