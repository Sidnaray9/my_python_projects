# my_python_projects
A repository for my independent python projects 

## E - Commerce Customer Segmentation Project

E-commerce Customer Segmentation and Prediction – Project Summary
In this project, I performed comprehensive customer segmentation and behaviour prediction based on an e-commerce dataset containing transactional records.

### 1. Data Preparation & Cleaning
I started by loading the data and exploring its structure. The data was segmented at two levels — customer (CustomerID) and transaction (InvoiceNo). I handled missing values, specifically addressing the 24.93% of entries with missing CustomerID. I analysed these separately, observing trends such as lower quantities and higher unit prices, suggesting they were special cases like online orders or returns.

---

### 2. Exploratory Data Analysis (EDA)
Using descriptive statistics and visualisations, I analysed customer behaviour patterns, purchasing frequency, unit prices, and returns. Special attention was given to patterns in InvoiceNo and StockCode for transactions without CustomerIDs.

---

### 3. Feature Engineering
I created several features to better represent customer behaviour:

RFM (Recency, Frequency, Monetary) values

Average Order Value

Customer Loyalty Duration

Returns Ratio

Total Purchase and Return Value

Product Categories purchased and most common items

---

### 4. Dimensionality Reduction
To facilitate visualisation and clustering:

I applied Principal Component Analysis (PCA) to reduce high-dimensional features into principal components while preserving variance.

I also used t-SNE (t-distributed Stochastic Neighbour Embedding) for non-linear dimensionality reduction and visualisation of complex patterns in 2D space.

---

### 5. Customer Clustering
I experimented with multiple clustering algorithms:

KMeans Clustering – Chosen as the final model for its interpretability and performance.

DBSCAN – Applied to discover density-based clusters, though less effective due to varying densities.

Hierarchical Clustering (AgglomerativeClustering) – Used to understand nested relationships between customer segments and visualised via dendrograms.

Cluster results were visualised using scatter plots (PCA and t-SNE transformed), providing business insight into customer groups based on behaviour and value.

---

### 6. Predictive Modelling
I built classification models to predict the cluster labels:

Random Forest Classifier – Delivered the highest accuracy and interpretability, with feature importance plots indicating which behaviours were most predictive.

Support Vector Machine (SVM) – Used for comparison but less effective than Random Forest.

Certainly! Here's the same report without any bold text formatting:

---

### 7. Interpreting Customer Segments from a Business Perspective

After applying clustering algorithms and visualising the results using PCA and t-SNE, I interpreted the clusters to uncover the distinct behavioural patterns of each segment. Each cluster represents a unique customer profile with different engagement levels, spending behaviours, and purchase frequencies.

- Cluster 0 (Purple) represents older customers who haven’t made recent purchases but previously engaged with frequent, smaller orders. Their current inactivity makes them ideal candidates for re-engagement efforts.

- Cluster 1 (Yellow) consists of high-value customers who are both recent and active buyers. They exhibit high average order values and contribute significantly to total revenue. Retaining this group is vital for long-term profitability.

- Cluster 2 (Green) includes moderately engaged customers with relatively lower spending. They are more recent than Cluster 0 but not as involved as Cluster 1. They show potential for growth with the right nudges.

This interpretation helped me align the segments with real-world business strategies tailored to maximise engagement and revenue from each group.

---

### 8. Recommended Engagement Strategies for Each Customer Segment

To leverage the insights drawn from customer segmentation, I proposed targeted business strategies tailored to the specific needs and behaviour of each cluster.

#### Cluster 0 (Purple) – Re-engagement Strategy

These are lapsed customers with a history of frequent but small purchases. The focus for this group is reactivating interest and reigniting purchasing behaviour.

- Reactivation Campaigns: I would deploy email campaigns with personalised messages, showcase new arrivals, and offer limited-time discounts or free shipping.

- Loyalty Incentives: Introduce a “Comeback Bonus” loyalty scheme where returning customers earn extra points for their next purchase.

- Content-Based Outreach: Create tailored content such as product guides or nostalgic campaigns referencing past purchases.

- Feedback Loop: Circulate surveys to understand why engagement declined and use these insights to improve offerings and communication.

#### Cluster 1 (Yellow) – Retention and Upselling Strategy

This cluster contains loyal, high-spending customers. The goal is to enhance their experience, reward loyalty, and encourage upselling.

- Personalised Offers: Use purchase history data to recommend relevant products and provide early access to sales or exclusive bundles.

- Loyalty Tiers and Referrals: Implement a premium rewards programme with escalating benefits. Encourage referrals through incentive-based schemes.

- Premium Services: Offer faster shipping, priority support, and tailored shopping experiences to make them feel valued.

- Cross-Selling Opportunities: Promote complementary items post-purchase or introduce subscription models for products they buy regularly.

#### Cluster 2 (Green) – Growth and Engagement Strategy

This group includes moderate-value customers who need nudging to increase their purchase frequency and order value.

- Incentives to Spend More: Provide discounts for orders above a certain value and promote bundled deals to encourage larger baskets.

- Content Education: Use informative content like product tutorials or comparisons to help customers understand value and explore additional offerings.

- Prompt Repeat Purchases: Send reminders and limited-time deals aligned with past purchase behaviour to increase repeat engagement.

- Leverage Social Proof: Encourage reviews and share testimonials to build trust and encourage further exploration.

- Behavioural Targeting: Use retargeting ads for cart abandonment or site visits to re-capture their attention.

---

### Strategic Recommendations Across Segments

- Segment-Specific Communication: I would develop distinct messaging strategies for each cluster using email, retargeting ads, and social media, aligned with their behaviour and value.

- Customer Journey Mapping: By mapping the typical journey of each segment, I can optimise touchpoints and create tailored interventions that improve conversion and experience.

- Data-Driven Strategy Refinement: I plan to regularly analyse customer behaviour and A/B test different offers to continuously improve engagement strategies.

- Continuous Feedback Loop: Finally, I would set up mechanisms for customers to provide feedback, allowing me to keep strategies customer-centric and responsive.



