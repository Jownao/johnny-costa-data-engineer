# Project Portfolio — Johnny Costa

This document presents selected data projects, structured to highlight decision-making, architecture choices, and business impact.  
The focus is not only on technical implementation, but on the reasoning behind each solution.

---

## 📌 Case 1 — Crypto Data Pipeline & Dashboard  
🔗 https://github.com/Jownao/crypto-dashboard  

### Problem  
Tracking cryptocurrency prices and metrics was a manual and fragmented process, leading to low reliability and significant time spent on data collection.  
Additionally, there was no structured historical dataset available for deeper analysis.

### Decision  
I chose to build an automated data pipeline in Python, consuming external APIs and storing data in analytical formats (CSV and Parquet).  

The key decision was **not to use a streaming architecture** (e.g., Kafka), prioritizing:
- lower operational complexity  
- zero infrastructure cost  
- faster implementation  

I also defined a **lightweight batch ingestion strategy**, balancing data freshness with API consumption limits.

### Result  
- Automated and scheduled data pipeline  
- Structured dataset ready for analysis  
- Consolidated historical price data  

### Impact  
- Estimated **80% reduction in manual data collection effort**  
- Creation of a reliable data foundation for analysis  
- Enabled future evolution into dashboards and predictive models  

---

## 📌 Case 2 — Steam ETL Pipeline  
🔗 https://github.com/Jownao/steamDbETL  

### Problem  
Steam data was available in raw and unstructured formats, making it difficult to analyze pricing, popularity, and trends across games.

### Decision  
I developed a modular ETL pipeline in Python, focusing on clear separation of stages (extract → transform → load).  

The main decision was to **avoid monolithic scripts** and instead design a reusable pipeline, prioritizing:
- maintainability  
- code reuse  
- clarity in data flow  

I also prioritized **data cleaning and standardization during the transformation stage**, reducing the need for rework during analysis.

### Result  
- Structured and reusable ETL pipeline  
- Clean and standardized dataset  
- Data ready for analytical use  

### Impact  
- Approximate **60% reduction in data preparation rework**  
- Significant improvement in data quality  
- Reusable foundation for future data projects  

---

## 📌 Case 3 — AWS S3 Data Pipeline  
🔗 https://github.com/Jownao/aws-second-s3  

### Problem  
There was a need to move from a local environment to a more production-like architecture with scalable and organized data storage.

### Decision  
I implemented AWS S3 as a data lake storage layer, organizing data using best practices for structure and partitioning.  

The key decision was to **prioritize simplicity and foundational cloud learning**, instead of adopting a more complex architecture involving multiple AWS services (e.g., Glue, Lambda).  

I also structured the data into logical layers (e.g., raw and processed), preparing the pipeline for future scalability.

### Result  
- Data lake structure implemented in AWS S3  
- Organized datasets with logical layering  
- Integration with existing pipeline processes  

### Impact  
- Hands-on experience with cloud-based data architecture  
- Improved readiness for real-world data engineering scenarios  
- Scalable foundation for handling larger data volumes  

---

## 📌 Case 4 — GenAI Application with Streamlit  
🔗 https://github.com/Jownao/genai_streamlit  

### Problem  
Exploring generative AI applications required a simple way to interact with models, without relying on complex backends or interfaces.

### Decision  
I built an application using Streamlit to enable rapid prototyping and user interaction.  

The main decision was to **prioritize speed and usability**, instead of developing a full-scale production application.  

I focused on creating a simple interface to validate user interaction with generative AI before optimizing the architecture.

### Result  
- Functional application with interactive UI  
- Integration with generative AI models  
- Direct user interaction experience  

### Impact  
- Reduced barrier to using generative AI (from code to interface)  
- Faster experimentation cycles with AI models  
- Foundation for future evolution into more robust applications  

---

## 📊 Final Considerations  

These projects reflect growth in:

- Data Engineering (ETL, pipelines, data modeling)  
- API integration  
- Cloud architecture (AWS S3)  
- Data structuring for analytics  
- Generative AI applications  

More importantly, they demonstrate a focus on:

- Context-driven decision-making  
- Trade-offs between complexity and value  
- Clear problem-solving approaches  
- Delivering practical impact  

---

📎 LinkedIn: https://www.linkedin.com/in/johnnywilliam/  
📎 GitHub: https://github.com/Jownao