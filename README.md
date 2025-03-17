# AWS-Data-Engineer-Notes

## Module 2- Data-Driven Decisions
### More Valuable insights are more difficult to derive
Less Valuable ---> More Valuable  
Descriptive --> Diagnostic --> Predictive --> Prescriptive  
**Descriptive**: What happened?  
**Diagnostic**: Why did something happened?  
**Predictive**: What will happen?  
**Prescriptive**: How can we make something happen or prevent from happening?  

The value of data for decision-making decreases over time, with the highest value in near real-time for preventive/predictive purposes, moderate value within hours for proactive insights, lower value within days for diagnostic analysis, and the lowest value being in historical data within days to months.  

## Simple Data Pipeline
Extracting Data from Data sources --> Data Wrangling tasks like discovering, cleaning, normalizing, enriching --> The wrangled data is tranformed into required format --> Stored & Processed for further use --> Analysis & Visualization --> Evaluating the previous steps --> Predictions & Decisions.  

### Common Data pipeline questions
For Data Engineer,  
Does the organization have the data that addresses the need? Where is the data stored and in what format?  
Will I need to combine data from multiple sources?  
What is the type and quality of data? What will be the source of truth?  
What are the security requirements for this data? Who needs access to it and in what state?  
What types of mechanisms are needed to transfer the data from its locations into the pipeline?  
How much data is there, and how frequently is it updated or processed?  

For Data Scientist,  
What can the data tell me?  
How will I evaluate the results?  
What kind of visualization do I need?  
Which formats and tools are the analysts familiar with?  
Do I need a big data framework?  
Which type of AI/ML models fit?  
What is the simplest way to implement AI/ML?  

### The role of Data Engineer 
Both data scientist roles and data engineering roles work with the data pipeline, and tasks might be performed by someone in either role.  
Data engineering is primarily focused on the infrastructure that the data passes through while the data scientist works with the data in the pipeline.  
To build the right pipeline, you need to ask questions about the desired outcomes and the data and then iterate on your answers as you learn more.  

## Module 3 - The Elements of Data

### Data Characteristics that drive infrastruture decision
The 5 V's of Data  
**Volume**: How big is the dataset And how much new data is generated?  
**Velocity**: How frequently is the new data generated and ingested?  
**Variety**: What types and formats? How many different sources does the data come from?  
**Veracity**: How accurate, precise and trusted is the data?  
**Value**: What insights can be pulled from the data?  

Most resources are put to get the best value from the data.  

### Volume and Velocity  
a) Volume is about how much data is needed to process.  
b) Velocity is about how quickly data enters and moves through the pipeline.  
c) Volume and Velocity together drive the expected throughput and scaling requirements of the pipeline.  
d) It is important to evaluate the volume and velocity requirements for each layer in the pipeline.  

**Scale the pipeline for volume and velocity of data**  
Scaling is important to handle data ingestion and storage at the pace of arrival.  
Consider how long data should be stored to balance cost and availability.  
To address a business problem we need to understand the amount data is needed to be processed and how quickly too.  
How frequently the data must be incorporated as consumers may need to access the data.  

**Ingestion**  
a) Streaming Ingestion: Continual ingestion of data that is needed to be processed as quickly as possible.  
b) Batch Ingestion: Periodical ingestion of data that is stored to process in batch.  

### Variety - data types 
a) Variety in data includes structured, semi-structured, unstructured.  
b) Structured data is the easiet to query but the least flexible.  
c) Unstructured data is the hardest to query but the most flexible.  

### Vairety - data sources
a) Databases and files owned by the company itself; It is often structured data.  
b) Public datasets available from various sources; It is often semi-structured data.  
c) Data generated from events, devices, sensors continually and includes time based component; It is mostly time-series data.  

### Veracity & Value  
a) Data integrity crucial as it may be combined with various data from different sources.  
b) Making data-driven decisions with bad data is much worse than limited or no data.  
c) The steps of ingestion, storage and processing play vital role in maintaining veracity of the data.  

**Examples of data issues that decrease veracity**  
a) Discover the following 
- Dated information
- Missing data
- Lack of lineage
- Ambiguity
- Statistical bias

b) Cleaning the data
- Duplicates
- Abnormalities
- Difference in source

c) Prevent
- Software bugs
- Tampering
- Humnan error

Value relies on veracity as good quality data is required for making good decisions.  

### Evaluating the Veracity of Data
---
### Data Engineering-Focused Questions:
- How is the source managed and maintained?
- Who generated the data, and who owns it?
- How often is the data updated?
- Do we need all fields and all records?
- Do audit trails exist?
---
### Data Science-Focused Questions:
- What methods were used to collect and process the data?
- Is this dataset the product of scientific research methods?
- What type of bias is likely part of this dataset?
- Does the data appear to be complete?
- How recent is the most recent data? Are there time gaps?
---
This checklist is essential for ensuring that your data sources are reliable and suitable for analytics and decision-making.

### Best way for cleaning the data  
- What is cleaning in your dictionary? Fiil null? Normalize the dataset? Or keep it raw?  
- Tracing the source of errors in data for data integrity.  
- Make changes in the dataset after careful consideration.  
- Valuable Raw data shouldn't be affected after data cleaning.  

Transformation includes changing data according to certain standards.  
Advanced transformation includes filtering records, joint operations, splitting columns, aggregating rows and data validation.  

### Maintaining Data Integrity and Consistency

**Key Principles for Ensuring Data Reliability:**
- **Secure all layers of the pipeline.**
- **Grant least privilege access.**
- **Apply best practices to maintain data integrity.**
- **Keep audit trails.**
- **Implement data compliance and governance processes**, including:
  - Data classification
  - Data cataloging
- **Maintain a single source of truth.**

---

This checklist is essential for maintaining high standards of data quality and ensuring that your systems and workflows remain robust and secure.

# Module Summary

This module equips you with essential knowledge to navigate data pipelines effectively. Here's what you'll learn:

---

## Key Learning Objectives:
- **Five Vs of Data:** Understand the foundational characteristics that define data.
- **Impact of Volume and Velocity:** Explore how data volume and velocity affect data pipelines.
- **Data Types:** Compare and contrast structured, semistructured, and unstructured data.
- **Common Data Sources:** Identify sources typically used to feed data pipelines.
- **Data Veracity:** Learn how to pose questions that assess the reliability of data.
- **Improving Data Integrity:** Discover methods to enhance the veracity of your data pipeline.

---

This summary serves as a guide to enhance your understanding of data pipelines and improve data quality in your workflows.
