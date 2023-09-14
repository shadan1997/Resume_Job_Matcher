  Resume_Job_Matcher  

  Approach 1: Cosine Similarity  
-   Objective  : Build a PDF extractor to extract details from CVs and match them against job descriptions.
-   Steps  :
    1. Data Preparation and Setup:
        - Import necessary libraries (NumPy, pandas, etc.).
        - Define the project objective and install required libraries.
        - Create a `cleanResume` function for text preprocessing.
    2. Job Description Dataset:
        - Load job descriptions from a CSV file and clean them.
        - Aggregate job descriptions by title.
    3. Testing on a Small Set:
        - Import additional libraries (pdfplumber, torch, cosine_similarity, etc.).
        - Preprocess text using DistilBERT.
        - Select a small set of job descriptions and CVs.
        - Calculate cosine similarity scores and rank CVs.
    4. Generating CSV for PDF Paths:
        - Create a CSV file with PDF file paths.
    5. Setting Up PDF Paths for Matching:
        - Define limits and load PDF paths.
    6. Applying Matching to All Categories:
        - Calculate cosine similarity scores for all job descriptions.
        - Rank and display top CVs.
    7. List of CVs:
        - Display CVs with file paths and indices.

-   Summary  : This project involves data preparation, text cleaning, and cosine similarity calculations to efficiently match CVs with job descriptions. It processes a large number of CVs and job descriptions to find relevant matches.

[GitHub Repository](https://github.com/shadan1997/Resume_Job_Matcher/blob/main/resume-job-matcher.ipynb)

  Approach 2: Frequency (TF-IDF)  
-   Objective  : Classify text data into categories (job descriptiom) using TF-IDF and machine learning models.
-   Datasets  :
    1. Resume Data:
        - Clean and encode resume text using TF-IDF.
        - Train a K-Nearest Neighbors classifier.
    2. Job Description Data:
        - Clean and encode job description text using TF-IDF.
        - Train a Random Forest Classifier for category prediction.
    3. Result for Job Descriptions:
        - Predict job categories for given descriptions.
-   Libraries  : pandas, numpy, nltk, scikit-learn, pdfminer.six.

[GitHub Repository] ( https://github.com/shadan1997/Resume_Job_Matcher/blob/main/task_resume_idf.ipynb)

  Approach 3: Applying Algorithm  
-   Algorithm  : GradientBoostingClassifier.
-   Accuracy  : 76%.

[GitHub Repository] (https://github.com/shadan1997/Resume_Job_Matcher/blob/main/GradientBoostingClassifier_model_76.ipynb)

These approaches demonstrate text processing, classification, and matching techniques for resumes and job descriptions. Approach 1 focuses on cosine similarity, while Approach 2 uses TF-IDF and machine learning models for classification.
