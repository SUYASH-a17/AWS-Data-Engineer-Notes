# AWS-Data-Engineer

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
- Volume is about how much data is needed to process.
- Velocity is about how quickly data enters and moves through the pipeline.
- Volume and Velocity together drive the expected throughput and scaling requirements of the pipeline.
- It is important to evaluate the volume and velocity requirements for each layer in the pipeline.

### Variety
- Variety in data includes structured, semi-structured, unstructured.
- Structured data is the easiet to query but the least flexible.
- Unstructured data is the hardest to query but the most flexible.
