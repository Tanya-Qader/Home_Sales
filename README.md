# Big Data - Home Sales Analysis

![image](https://user-images.githubusercontent.com/116117065/231039411-2289f888-4bfb-43c4-9c31-cf3e59a3a582.png)

### What is Big Data?

Big data is a term used to describe extremely large and complex data sets that are difficult to manage and analyze using traditional data processing tools and techniques. These data sets are typically characterized by the volume, velocity, and variety of the data being generated, which can come from a wide range of sources, including social media, sensors, machines, and other digital devices. The term "big data" also refers to the technologies and practices used to store, manage, and analyze these data sets, which often require specialized hardware and software tools. The goal of big data analysis is to extract valuable insights and knowledge from these large data sets, which can help organizations make better decisions, improve their operations, and gain a competitive edge in their industries.

### What is Apache Spark?

Apache Spark is an open-source, distributed computing system this is designed to process and analyze large datasets in a parallel and fault-tolerant manner. 
Spark also provides a range of libraries and APIs for machine learning, graph processing, stream processing, and SQL-based data analysis.
Spark is built around the concept of Resilient Distributed Datasets (RDDs), which are fault-tolerant collections of objects that can be processed in parallel across a cluster of machines. 


In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Instructions

1. Import the necessary PySpark SQL functions for this assignment.
2. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
3. Create a temporary table called home_sales.

4. Answer the following questions using SparkSQL:
    * What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
    
    ![image](https://user-images.githubusercontent.com/116117065/231318073-73c849aa-d9e7-406d-b9b1-d3be1d804a91.png)


    
    
    * What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
    
    ![image](https://user-images.githubusercontent.com/116117065/231318160-2cc4d9c3-d937-413e-b06a-d85a60b313b2.png)


    
    
    * What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
    
  ![image](https://user-images.githubusercontent.com/116117065/231318263-b626081b-e5e9-45e6-95a6-8618fb45353a.png)


    
    
   * What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
    
   
   ![image](https://user-images.githubusercontent.com/116117065/231318382-58df92fa-e656-4da7-a0a5-bf6f6b5e27bb.png)





6. Cache your temporary table home_sales.
7. Check if your temporary table is cached.
8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![image](https://user-images.githubusercontent.com/116117065/231318696-73546d95-dde3-4dcd-b846-a5ab41eb646d.png)



9. Partition by the "date_built" field on the formatted parquet home sales data.
10. Create a temporary table for the parquet data.
11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![image](https://user-images.githubusercontent.com/116117065/231318636-6e51c9f4-baba-4788-af92-6b77a82e23f3.png)



12. Uncache the home_sales temporary table.
13. Verify that the home_sales temporary table is uncached using PySpark.
