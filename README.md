# Sales Method Analysis and Optimization

## **Description**  
This project validates, cleans, and analyzes a dataset containing 15,000 rows of customer sales data. The goal is to evaluate the performance of three sales methods—**Email**, **Call**, and **Email + Call**—and provide actionable insights to improve business strategies. Using both R and SQL, the data has been processed to extract trends, calculate metrics, and visualize revenue distribution.

---

## **Table of Contents**  
1. [Data Validation](#data-validation)  
2. [Analysis](#analysis)  
   - [Customer Distribution by Approach](#customer-distribution-by-approach)  
   - [Revenue Spread](#revenue-spread)  
   - [Revenue Trends Over Time](#revenue-trends-over-time)  
3. [Recommendations](#recommendations)  
4. [Business Metrics](#business-metrics)  
5. [Visualizations](#visualizations)  
6. [How to Use](#how-to-use)  
7. [Tools and Technologies](#tools-and-technologies)  
8. [Future Enhancements](#future-enhancements)
9. [Presentation preview](https://www.datacamp.com/datalab/w/c7abc379-99aa-45be-868f-fb402ffaf43c)) 

---

## **Data Validation**  
The initial dataset contained 15,000 rows and 8 columns. Key cleaning steps included:  
- Converting revenue to numeric format and removing invalid values.  
- Standardizing `sales_method` into three categories: Email, Call, Email + Call.  
- Correcting outliers in `years_as_customer` to match the company's founding year (1984).  
- Ensuring revenue values are rounded to two decimal places.  

### **Before Cleaning**  
- Total records: **15,000**  
- Invalid `revenue` rows: **1,074**  
- Inconsistent `sales_method` entries: Found across 5 unique values.  

### **After Cleaning**  
- Total valid records: **13,926**  
- Standardized columns: `sales_method`, `revenue`, and `years_as_customer`.  

---

## **Analysis**  

### **Customer Distribution by Approach**  
- **Email**: 6,922 customers (49.7%).  
- **Call**: 4,781 customers (34.3%).  
- **Email + Call**: 2,223 customers (16.0%).  

Email dominates due to its efficiency and scalability, while Email + Call engages fewer customers but generates higher revenue per interaction.

---

### **Revenue Spread**  
- **Overall Statistics**:  
  - Min: $32.54 | Max: $238.32  
  - Mean: $93.93 | Median: $89.50  
  - Standard Deviation: $47.43  

- **By Method**:  
  - **Call**: Avg. revenue $47.6 (range: $32.5–$52.7).  
  - **Email**: Avg. revenue $97.1 (range: $78.8–$105).  
  - **Email + Call**: Avg. revenue $184.0 (range: $122–$238).  

---

### **Revenue Trends Over Time**  
- Weekly trends reveal:  
  - **Email**: Stable revenue ($90–$100) with minimal variation.  
  - **Call**: Consistently low revenue ($40–$50).  
  - **Email + Call**: High revenue ($150–$190) with significant week-to-week variability.  

---

## **Recommendations**  

### **Primary Recommendation**  
Adopt **Email** as the primary sales method due to:  
- High efficiency ($1,142.76/hour).  
- Minimal time investment (5 minutes/customer).  
- Scalability and consistent performance.  

### **Secondary Strategy**  
Utilize **Email + Call** for high-value opportunities, as it offers the highest revenue per interaction ($184.0).  

### **Discontinue Call Method**  
The standalone Call method generates the lowest revenue and has poor time efficiency ($93.56/hour).  

---

## **Business Metrics**  

- **Revenue per Customer Contact (RPC)**:  
  - Email: $95.23  
  - Call: $46.78  
  - Email + Call: $175.45  

- **Resource Efficiency Ratio (RER)**:  
  - Email: $1,142.76/hour  
  - Call: $93.56/hour  
  - Email + Call: $701.80/hour  

- **Customer Response Rate (CRR)**:  
  - Email: 49.7%  
  - Call: 34.3%  
  - Email + Call: 16.0%  

---

## **Visualizations**  
The following visualizations were created using **R (ggplot2)**:  
1. **Customer Distribution by Sales Method**:  
   - Bar plot showing the proportion of customers using each method.  

2. **Overall Revenue Distribution**:  
   - Histogram highlighting the spread of revenue across all methods.  

3. **Revenue by Method**:  
   - Box plots and density plots showing revenue patterns for each method.  

4. **Weekly Revenue Trends**:  
   - Line chart depicting average revenue per week for each method.  

