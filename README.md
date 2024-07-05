# Blog Recommendation System

## Overview
This project focuses on building a Blog Recommendation System tailored for users involved in online competitive programming communities. We utilized the Codeforces blogs dataset, which was scraped using a Selenium script. The project involves leveraging advanced natural language processing (NLP) techniques and machine learning algorithms to provide personalized blog recommendations.

## Team Members
- IMT2021010 Raj Bunsha
- IMT2021080 Pannaga Bhat
- IMT2021095 Kadaru Jashwanth Reddy

## Instructor
- Prof. Raghuram Bharadwaj

## Objectives
- Scrape and construct a dataset from Codeforces blogs.
- Implement various recommendation methodologies.
- Evaluate the effectiveness of the recommendation models using relevant metrics.

## Dataset Description

### Dataset Construction
- The dataset was constructed using a combination of the Codeforces API and web scraping techniques with Selenium.
- Over 40,000 blogs were collected, focusing on diverse topics within the competitive programming domain.

### Data Overview
- The dataset comprises various attributes for each blog entry, including user, title, tags, and net upvotes/downvotes.

### Preprocessing & EDA
- Data cleaning and exploratory data analysis (EDA) were performed to gain insights into the dataset's distribution and characteristics.

## Methodology & Approaches

### Methodology 1: Blog Vector Representation

1. **Representing Blogs as Vectors**
   - Techniques used: SpaCy, Gensim's Doc2Vec, BERT model.
   - Cosine similarity was calculated to find the most similar blogs to the user representation.

2. **PCA for Better Representation and Clustering**
   - Principal Component Analysis (PCA) was used to reduce dimensionality and extract latent features from the blog vectors.

3. **User Representation**
   - Initial user representation was the average of all liked blogs.
   - KMeans clustering was used to form centroids representing user likes, resulting in a set of vectors for user representation.

### Methodology 2: Topic Modelling and MAB

1. **Topic Modelling Using N-grams + LDA**
   - Blogs were represented as a bag of n-grams and processed using LDA (Latent Dirichlet Allocation) to label blogs with topic numbers.

2. **Multi-Armed Bandit (MAB) - Upper Confidence Bound (UCB)**
   - MAB was used to make batch recommendations and simulate user interactions.
   - The UCB method calculated rewards associated with each topic, balancing exploration and exploitation.

## Sample Results
- **Input:** Sample blogs liked by the user.
- **Output:** Top recommendations using BERT, Gensim, and SpaCy models.

## Evaluation of Models

### Evaluation Metrics
- Precision, recall, and mean average precision (MAP) were used to evaluate model performance.
- Both overall and user-specific recommendations were considered.

### Results
- The recommendation models demonstrated high precision and recall scores.
- User feedback and interaction data further refined the recommendations over time.

## Conclusion
This project successfully developed a blog recommendation system for competitive programming communities. By leveraging advanced NLP techniques and machine learning algorithms, personalized and relevant blog suggestions were provided, enhancing the user experience on platforms like Codeforces.


## References
- AI-705: Recommendation Systems Final Report
- [Project Report](./RS_Final_Report_IMT2021095_080_010.pdf)  (Add the correct path to your report file)

## Contact
For any queries or further information, please contact [Jashwanth.Kadaru095@iiitb.ac.in].
