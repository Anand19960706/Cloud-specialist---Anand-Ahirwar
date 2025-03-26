data-analysts-anand

 👋 Hi, I'm Anand Ahirwar  
📊 Data Analyst | 🔍 EDA | 🛠️ Data Wrangling | 📈 Data Visualization
Doing MBA in Business but Major in Business anlytics and cloud computing, data understanding. 

Welcome to my GitHub portfolio!  
Here, you'll find a collection of my data analysis projects, showcasing my skills in exploratory data analysis (EDA), data wrangling, and visualization using Python, SQL, Tableau, and Power BI.  

✨ I’m passionate about transforming raw data into meaningful insights to drive better decision-making. Feel free to explore my projects, and don’t hesitate to reach out if you have any questions or collaboration ideas!

📫 Connect with me:  
💼 [LinkedIn]-www.linkedin.com/in/anand-ahirwar
  
📧 [Email]-ahirwar.anand96@gmail.com 



AWS - Amamzon web services 


i took City vancouver DATA of BUildiing Permit Issued Till now , it includes permit number , property location and many more features. 

DAP Design and Implementation and Descriptive Analysis

Project overview  - This analysis aims to track changes in number of building permits issued. This analysis helps understand how many permits are issued and what is the issue date, created date , applicant name , years of issue ,  address of the building and etc.  

The data analytic platform is designed based on four key components:


Data analytics platform (DAP) design – This is the road map for the whole AWS process which I have followed to land o the result i.e. Summarization technique



![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)


1.	Data Collection & Ingestion of  Building permit  dataset and uploading into S3 bucket.
2.	Data Profiling - Using AWS Glue DataBrew to from  structured  data.
3.	Data Cleaning - Using AWS Glue DataBrew to clean the data.
4.	Data Cataloging - Organizing the cleaned data into a well-defined schema using AWS Glue and storing it in AWS S3.( catalog file )
5.	Data Summarization - Running extraction, time stamp, filter, transform and loading into User and System format, using AWS Glue.





Data analysis diagram 
Vancouver city portal- Its shows value of the building permit issued between to year 2017 to 2015 and other Y- axis line shows permit elapsed days.  

![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/5924e14c44219b9bf82d6873152f4a9915ab9a98/image.png)





Data Collection & Ingestion -  

downloaded the data.csv (Permits_dataset.csv) from city of Vancouver portal. It is the big data all the permits issued by the city along with issue date, name of the applicant, type of property, value of the property, created date of the permit and other 10-15 columns related to building permit issue.


![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/35e3677fbb6d7d4dd8204b47da98cdf8919242d5/image.png)







Data Profiling - Using AWS Glue DataBrew to structure the data.
In this step, I analyse the quality of the data by checking for errors, missing values, and patterns. This helps me understand the structure and completeness of the data before using it for analysis. I created the new bucket in S3 by the name of van-city-trf-anand. After adding profiling job the file saved to van-city-trf-anand. 




![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/ee0a716aa30c781fa38d6fcb8e0cd941d915634b/image.png)


user output  

![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)




Data Cleaning - Using AWS Glue DataBrew


data cleaning like rename the column heading for easy understanding. 


![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/2d7280ad218c4f5339032bd1bcbd6b09cd2f5d4b/image.png?raw=true)



Data Cataloging - Organizing the cleaned data into a well-defined schema


I organize the data by creating a tabular format  data source. This makes it easier to locate and use relevant data when it’s in need .


![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)

Data Summarization

I summaries the data so that it is useful to make decision. a field and columns which are not required I removed them to make a concise report in the format of (.csv) for the user and (.parquet)  file for the system 

![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/8041933c60cff6eef4919a9bca928caa57d76bcc/image.png)



Final output of both the report for the user and system 





![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/56fc87f37b2bcf3084ccc89257abc1d95d1053d3/image.png)


user out put 


![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/18771e134ca1b5d2adcfab98d6cda96cf5f12fbe/image.png)





DAP Estimated Cost	Monthly cost(USD)	Total 12 months cost(USD)
Team member 2
Data Cleaning & Data Summarization	3.10*12 
(month*12) 	37.20USD
		

AWS price estimator 


![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/d92cb067ecd5d76d609608ca210e1721dea57e19/image.png)




Now i am going to apply some more procedure on the Van city data to make it more usefull information Out of it. 




The implementation of the Data Analytics platform is done in four phases.


1.	Data Analysis: Using AWS Glue to create a Data Catalog and the business questions using SQL.
2.	Data Security: Using the AWS Key Management Service (KMS) for encryption of the buckets in the AWS S3 Bucket.
3.	Data Governance: Using AWS Glue to create a pipeline that examines the data quality and saves the result in the AWS S3 Buckets. 
4.	Data Monitoring: Using AWS CloudWatch and AWS CloudTrail to keep track of data security and monitor performance and integrity to identify operational failures and unauthorized access as well as inefficiencies for continuous operations that adhere to AWS governance policies.


data analytics platform for the City of Vancouver
(DAP Daigram)


![image](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)



Figure-2  data set was relational but still  I made sure that is should be relational and single source of truth . So dataset transfer to user and system for further usage , for the user I maintained the CSV file and for the system easy usage set the output in parquet file.   

(User output structed data)

![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/617cfbf5526183d1a283d32951314afbcb523f2b/image.png)




I run the business question query – what is the avg project value of the van city projects of building ( in includes residential and commercial)


![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)






Now I applied the data security measure by creating the KMS key which help to protect the data. 



![image.alt](<img width="452" alt="image" src="https://github.com/user-attachments/assets/9684ca70-e1dd-4219-a812-976996eef04d" />
)

