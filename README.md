***Pyspark assignment***

***Deploy a Spark Cluster (standalone, single node is quite sufficient) in local machine***

***Pyspark Installlation Guides***

Install Apache Spark on Windows

Step 1: Install Java jdk : url =  https://java.com/en/download/.

Step 2: Install Python : url =  https://www.python.org/

Step 3: Download Apache Spark : url = https://spark.apache.org/downloads.html

Step 4: Install Apache Spark  : 
        if you download .tgz extract it place in c drive with folder name spark 
        
        
Step 5: Add winutils.exe : url = https://github.com/cdarlint/winutils  :
        Paste File in spark location bin folder 
        
        
Step 7: Configure Environment Variables

Step 1- Set the environment variables : 
            Now, we need to set few environment variables which are required in order to set up Spark on a Windows machine. 
            
            Set SPARK_HOME = "C:\Spark\spark-2.4.3-bin-hadoop2.7"
            
            Set HADOOP_HOME = "C:\Spark\spark-2.4.3-bin-hadoop2.7"
            
            Set JAVA_HOME = "C:\Progra~1\Java\jdk1.8.0_212"
            
            Set PYTHON_HOME = "C:\Progra~1\Python\Python310\"
    
Step 2 – Update existing PATH variable :

         Modify PATH variable to add:
            
         C:\Progra~1\Java\jdk1.8.0_212\bin
            
         C:\Spark\spark-2.4.3-bin-hadoop2.7\bin
            
Step 3 – Update py4j pyspark library PATH variable :

         PYTHONPATH = %SPARK_HOME%\python;%SPARK_HOME%\python\lib\py4j-0.10.9-src.zip;%PYTHON_HOME%

Step 8 : pip Install pyspark

Step 10 : Run Spark code


***Creating a Notebook tp Analyse the data-set***


#Load the dataset from the link
(https://www.kaggle.com/promptcloud/careerbuilder-job-listing-2020) using Spark inside the job


***Apply the following transformation on top of the data***
    
#1 calculate number of jobs posted on daily basis, per each city

#2 calculate average salary per job title and state

#3 identify the top 10 most active companies by number of positions opened

#4 create a UDF function to clean job description from HTML code contained inside analyze and comment on the performance of the UDF function.

#5 How the performance could be improved

***Export the results of each analyses to a CSV file***
