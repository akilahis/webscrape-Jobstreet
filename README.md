# 📊 Malaysia Job Market Analysis For 'Data-Analyst' Role

A data analytics project to identify in-demand skills, salary trends, and employer preferences for data analyst roles in Malaysia. Project is executed for myself to thoroughly understand the job market for 'data-analyst' roles, thus optimizing my own job-seeking processes.

[![Python 3.8+](https://img.shields.io/badge/python-3.8%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🚀 FEATURES
- **Web Scraping**: Automated extraction of 1000+ active job listings during November 2024, from JOBSTREET MY website using keyword 'data-analyst'.
- **Skill Extraction**: NLP-powered keyword analysis to identify top tools (Python, Power BI) and skills.
- **Salary Trends**: Visualization of salary distributions by industry and job roles.
- **Machine Learning**: Clustering analysis to cluster jobs according to salary level (low, average, high). Classification analysis to classify and predict job listings according to salary level.

---
## ⚠️ CHALLENGES
**Data Availability**
- From 1280 job listings, only 23% (302 jobs listings) are advertised with salary ranges.
- From 1280 job listings, only 26% (338 job listings) mentioned specific tools required.

**Unstructured Job Description**
- Every job listings have unstandardized job description formats, making it difficult to extract relevant skills and qualifications. Further extensive text pre-processing is required. 

**Keyword Relevance**
- Results produced on the website may not always align with the intended keyword ('data analyst'). Towards end of the scraped pages, for example, some listings may include unrelated roles or ambiguous terms that may cause noises on the dataset. This may explain why some job listings had no mention of specific tools commonly required for analytics roles.

---

## 📉 INSIGHTS
### **1. Industries with highest demand for Data Analysts in Malaysia**
1. **Information & Communication Technology**  
2. **Accounting**  
3. **Banking & Financial Services**  
4. **Manufacturing, Transport & Logistics**  
5. **Science & Technology**  

### **2. Most In-Demand Tools**
From **338 job listings**, the most frequently mentioned tools are:
- **EXCEL**: 100% of job postings  
- **SQL**: 90% of job postings  
- **PYTHON**: 50% of job postings 
![image](https://github.com/user-attachments/assets/3ca035dc-efac-450c-8b38-77f189e47382)

### **2. Average salary according to job role (top 5 most advertised job role)**
    - Business/Systems Analysts, Average Salary: RM 6123
    - Analysis & Reporting, Average Salary: RM 5287
    - Database Development & Administration, Average Salary: RM 5784
    - Developers/Programmers, Average Salary: RM 5630
    - Digital & Search Marketing, Average Salary: RM 3060
  ![image](https://github.com/user-attachments/assets/cf2ad626-53e3-4f77-b635-ba56c21ad138)

### **3. Clustering analysis for salary level (Clusters : 0=high, 1=average, 2=low)**
![image](https://github.com/user-attachments/assets/cc2c1bfd-9ac4-4578-9003-c0422c525836)

### **4. Classification analysis to predict salary level for job listings**
- As mentioned, only 23% of jobs listings are advertised with salary ranges. Developing a salary predictive classifier model can address the lack of salary data in job listings. 
- Random Forest Classifier predict salary level with **60% accuracy**, using features such as job_role, job_sector, and states.
- Feature importance shows that **job_role is the most influential factor impacting salaries**.





