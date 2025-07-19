# 📚 Book Recommendation System using Big Data Technologies on AWS

> 🛠️ This project was implemented entirely on **AWS**, allowing us to showcase the full **workflow**, **pipeline**, and **processing steps** of building a large-scale recommendation system using real-world cloud infrastructure.

---

## 📌 Overview & Background

Our project, **"Book Recommendation System,"** is designed to help readers discover books that match their preferences using the **Amazon Book Reviews dataset**. By leveraging powerful **AWS services** such as:

- Amazon S3
- AWS Glue
- AWS Lambda
- Amazon SageMaker

We constructed a **scalable**, **automated**, and **hybrid recommendation engine** that integrates **machine learning** with **big data processing pipelines**.

---

## ❓ Problem Statement

Building a book recommendation system at scale presents several core challenges:

- 🔍 Extracting **meaningful insights** from vast volumes of **unstructured review data**.
- 🧠 Designing a system that **adapts to dynamic user preferences** and behaviors.
- ⚙️ Balancing **recommendation accuracy** with **computational efficiency** across large datasets.

---

## 📂 Dataset

- **Source**: Kaggle – Amazon Book Reviews  
- **Size**: ~1 GB  
- **Type**: JSON format with user reviews, ratings, book metadata

### 📸 Sample Data Preview  
![Dataset Sample](images/data_scheme.png)
![Dataset Sample1](images/data_ex1.png)
![Dataset Sample2](images/data_ex2.png)

---

## ☁️ Related Big Data Technologies on AWS

### 🗃️ Amazon S3  
Bucket: `rayong-book-bucket-g12`  
Used for storing raw datasets and intermediate results.

*(ใส่รูปหน้าจอ S3 Bucket)*  
`![S3 Screenshot](path/to/s3.png)`

---

### 🧬 AWS Lambda  
Function name: `rayong-lambda-g12`  
Used to automate ETL trigger, notifications, preprocessing, and model execution.  
Scripts:
- `glue_trigger.py`
- `notify.py`
- `preprocessing.py`
- `sagemaker_train.py`
- `lambda_function.py`

*(ใส่รูป Lambda function + code snippets หรือ GIF ทำงาน)*  
`![Lambda Screenshot](path/to/lambda.png)`

---

### 🔄 AWS Glue  
Job: `book-recommendation-etl`  
Performs data cleaning, feature extraction, and schema transformation.

*(ใส่รูปหน้าจอ Glue job + workflow)*  
`![Glue Screenshot](path/to/glue.png)`

---

### 🤖 Amazon SageMaker  
Trains and deploys the machine learning models.

#### 📗 Collaborative Filtering  
Recommends items based on **user behavior**.  
Two types:

- **User-Based CF**  
  > Uses similarity between users  
- **Item-Based CF**  
  > Uses similarity between items  

**Matrix-based approach** using user-item interaction.

*(ใส่รูปหรือ schema อธิบาย Collaborative Filtering)*  
`![Collaborative Filtering](path/to/cf_diagram.png)`

---

#### 📘 Content-Based Filtering  
Recommends items using **item metadata** and user history.  
Features:
- Description
- Authors
- Categories
- Sentiment Score (NLP)

Steps:
- Create item profiles using features
- Match user preferences to content vectors

*(ใส่รูปการทำ content-based filtering หรือ feature table)*  
`![Content-Based](path/to/cb_features.png)`

---

#### 🔀 Hybrid Approach  
Combines both Collaborative & Content-Based filtering.  
Advantages:
- More **personalized**
- Better **coverage**
- Reduced **cold-start problems**

*(ใส่ schema หรือภาพอธิบาย Hybrid Approach)*  
`![Hybrid Model](path/to/hybrid_model.png)`

---

## 📊 Tableau Visualization  
We used **Tableau** for visualizing results and data insights to support business intelligence (BI).

- User Review Trends
- Top Rated Books
- Genre Popularity
- Model Evaluation Metrics

*(ใส่ 4 รูป Tableau dashboard ที่ต่างกัน)*  


---

## 🧩 Workflow Summary  
> A complete end-to-end pipeline using AWS Big Data Ecosystem:

1. **Upload raw data** to S3
2. **Preprocess** with AWS Glue
3. **Trigger Lambda** to start ETL + training pipeline
4. **Train ML models** using SageMaker (Collaborative + Content-based)
5. **Generate recommendations**
6. **Visualize** results in Tableau

*(ใส่รูปภาพรวมของ architecture/workflow diagram หรือ GIF flow)*  
`![Pipeline Diagram](path/to/pipeline_diagram.png)`

---

## ✅ Key Features
- Real-time, scalable recommendation pipeline
- Uses hybrid recommender strategy
- Fully serverless infrastructure
- Clean, modular code structure

---

## 📎 Credits
Team G12 – Big Data for Business 2025  
Instructor: [Your Instructor Name]  
Dataset: Kaggle Amazon Book Reviews

---

## 📬 Contact  
For any questions or collaborations:  
📧 your.email@example.com

---


