AWS Cloud-specialist---Anand-Ahirwar

 👋 Hi, I'm Anand Ahirwar  


AWS Cloud-specialist|📊 Data Analyst | 🔍 EDA | 🛠️ Data Wrangling | 📈 Data Visualization
Doing MBA in Business but Major in Business anlytics and cloud computing, data understanding. 

Welcome to my GitHub portfolio!  

Here, you'll find a collection of my data analysis projects, showcasing my skills in exploratory data analysis (EDA), data wrangling, and visualization using Python, SQL, Tableau, and Power BI.  

 I am deeply passionate about cloud computing, with a particular fascination for Amazon Web Services (AWS). Ever since I first explored the world of cloud technology, I’ve been captivated by its limitless potential to revolutionize how businesses operate—making them more agile, scalable, and efficient. AWS, in particular, stands out to me because of its sheer versatility and dominance in the industry. The idea of building resilient, secure, and innovative solutions on the AWS platform excites me and drives my commitment to mastering its services.

I am especially drawn to AWS’s breadth of services—from foundational tools like Amazon EC2, S3, and RDS to cutting-edge solutions such as AWS Lambda, Elastic Kubernetes Service (EKS), and CloudFormation. The flexibility AWS offers in creating serverless architectures and automated deployments inspires me to dive deeper into its capabilities. I am eager to explore DevOps practices, leveraging AWS tools for continuous integration and delivery (CI/CD), infrastructure as code (IaC), and cloud security optimization.

My journey into AWS is not just about learning individual services—it’s about understanding how to design and implement holistic cloud solutions. I actively seek out hands-on experience through labs, projects, and certifications. My goal is to earn the AWS Certified Solutions Architect – Associate certification as a stepping stone toward becoming an expert in cloud architecture. This certification will validate my skills and reflect my dedication to building efficient, reliable, and scalable cloud systems.

What truly drives me is the realization that AWS is not just transforming technology—it is reshaping industries. The prospect of being part of this cloud-driven evolution, helping organizations innovate faster, reduce costs, and enhance security, genuinely excites me. I am determined to continuously expand my knowledge, staying ahead of industry trends and mastering the latest AWS innovations.

Ultimately, my ambition is to become a cloud solutions architect who not only builds secure and scalable infrastructures but also drives innovation and solves real-world challenges. I am excited to embark on this journey, fueled by an unyielding curiosity and a deep-seated passion for AWS and its transformative power.










📫 Connect with me:  
💼 [LinkedIn]-www.linkedin.com/in/anand-ahirwar
  
📧 [Email]-ahirwar.anand96@gmail.com 



AWS - Amamzon web services ( Detailed project on Vancouver city ( Building Permit issued by city)


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



![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/b053be7b1d7e9f9aa9734e207841080da9f44fe3/image.png)







In this process I applied Encryption using the above key which I made in pervious screenshot




![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)











in this I used the AWS Glue to check the quality of data, applied few filters like completeness, uniqueness and number of columns filter.  


![image.alt](https://raw.githubusercontent.com/Anand19960706/data-analysts-anand/44d00aa5aea284436cbfc01b8dbb511e18a05b90/image.png)








This is beautifully designed dashboard which shows allows to the user to monitoring parameters at one place , easy to keep eye on it. 


![image.alt](https://github.com/Anand19960706/data-analysts-anand/blob/main/image.png?raw=true)



