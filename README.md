# Home_Sales

![image](https://user-images.githubusercontent.com/116117065/231039411-2289f888-4bfb-43c4-9c31-cf3e59a3a582.png)


In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Instructions

1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.
2. Import the necessary PySpark SQL functions for this assignment.
3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.
4. Create a temporary table called home_sales.
5. Answer the following questions using SparkSQL:
    * What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
    
    ![image](https://user-images.githubusercontent.com/116117065/231040912-29122e5a-8b4e-4919-85b9-dcaa7825007e.png)

    
    
    * What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
    
    ![image](https://user-images.githubusercontent.com/116117065/231041015-f997b0c2-da89-45fe-b717-84dbd11d5cc5.png)

    
    
    * What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
    
    ![image](https://user-images.githubusercontent.com/116117065/231041070-da989794-fa0c-4a18-a426-61c7f4e6f2ab.png)

    
    
    * What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.
    
    ![image](https://user-images.githubusercontent.com/116117065/231041177-1fc1db0c-06b3-4c42-a199-197a3bc12e01.png)




6. Cache your temporary table home_sales.
7. Check if your temporary table is cached.
8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![image](https://user-images.githubusercontent.com/116117065/231041367-646f3c57-05bb-4edc-b9d3-d139bdaed80a.png)



9. Partition by the "date_built" field on the formatted parquet home sales data.
10. Create a temporary table for the parquet data.
11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
12. Uncache the home_sales temporary table.
13. Verify that the home_sales temporary table is uncached using PySpark.
14. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.
