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
figure no 3



![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)




Data Cleaning - Using AWS Glue DataBrew


data cleaning like rename the column heading for easy understanding. 


![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/2d7280ad218c4f5339032bd1bcbd6b09cd2f5d4b/image.png?raw=true)



