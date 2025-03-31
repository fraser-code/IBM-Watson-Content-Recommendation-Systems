# IBM Recommendation System

This project builds a Recommendation System for IBM's community platform. The goal is to suggest relevant articles to users based on using 3 different recommendation systems.
1) **Popularity-Based Recommendations**

Used for new users who have no reading history to base recommendations on. This approach simply recommends the most popular articles, typically measured by the highest number of views or interactions, ensuring that new users are presented with widely appreciated content.

2) **User-user collaborative recommendations**

Articles read by users who have similar reading patterns to our target user are recommended. In this method, cosine similarity is used to identify users with similar interests. We rank these users by similarity scores, review their article lists, and filter out articles that the target user has already read. This method helps in discovering articles that are popular among like-minded users, thus enhancing the recommendation's relevance.

3) **Content-based recommendations**

Articles similar to those a user has historically engaged with are suggested, utilizing advanced NLP techniques. The process starts with the creation of article vectors using a TF-IDF vectorizer, followed by dimensionality reduction via Latent Semantic Analysis (LSA) with Truncated SVD. To ensure optimal clustering, we apply the elbow method to determine the best number of clusters (k) and then use k-means clustering to group similar articles. This clustering helps in recommending articles that are content-wise similar to those the user prefers.

## Getting Started

Instructions for how to get a copy of the project running on your local machine.

### Dependencies

```
Python 3.11
Jupyter Notebook
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
```

### Installation

To set up the environment and run the project, follow these steps:

1) Clone this repository
```
cd path/to/your/directory
git clone https://github.com/fraser-code/IBM-Watson-Content-Recommendation-Systems
```
2) Open the Jupyter Notebook

3) Run all cells

## Built With

* [Pandas](https://pandas.pydata.org/) - Data Manipulation
* [Scikit-learn](https://scikit-learn.org/) - Machine Learning Algorithms
* [Matplotlib](https://matplotlib.org/) & [Seaborn](https://seaborn.pydata.org/)- Data Visualisation
