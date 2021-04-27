## Analyzing 10Gb of Yelp Reviews Dataset

Summary: Loading Yelp Reviews data from Kaggle to a Spark Cluster provisioned on AWS EMR and doing a few analyses

### 1. Install and Set Up Spark Cluster and Jupyter Notebook on AWS EMR
- Go to aws.amazon.com to sign in and look up EMR 
- Create a Cluster with specifications as below:

![Cluster Analysis](https://user-images.githubusercontent.com/55850536/116314674-66a87a00-a77d-11eb-8b7d-74cd3430de46.png)

- Then create a Notebook using the cluster that was created previously. Below is the Notebook Configuration:

![Notebook Configuration](https://user-images.githubusercontent.com/55850536/116313695-10870700-a77c-11eb-9fa7-263c98d21b47.png)


### 2. Upload Data to Amazon S3 Bucket
- Go to S3 on AWS and Create a bucket with a name
- Create a folder called "yelp/" then download 3 Yelp datasets from Kaggle (files ending "_user.json", "_review.json", "_business.json") 
- Upload these datasets to the S3 bucket 

### 3. Load Data to Spark and Run the Analysis
- Open the notebook in Jupyter Lab 
- Follow the code in Analysis.ipynb

### 4. Terminate the Cluster
- Make sure to terminate the cluster after being done with the analysis to avoid excessive cost
- Stop the notebook as well 
