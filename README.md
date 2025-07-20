# Movierecomandationsystem

**Overview**
This project implements a content-based movie recommendation system using Python. The system recommends movies to users based on the similarity of their "tags" (genres, keywords, cast, crew, and plot keywords) to a given movie. It leverages natural language processing (NLP) techniques like stemming and vectorization, followed by cosine similarity to determine movie similarities.

**Features**
Content-Based Filtering: Recommends movies based on shared attributes rather than user ratings or interactions.

Text Preprocessing: Utilizes NLTK's Porter Stemmer to reduce words to their root form, improving similarity matching.

Vectorization: Converts movie tags into numerical vectors using CountVectorizer from scikit-learn.

Cosine Similarity: Calculates the similarity between movie vectors to find the most similar movies.

Simple Recommendation Function: Provides a user-friendly function to get recommendations for a given movie title.

**Technologies Used**
Python

NumPy

Pandas

NLTK (Natural Language Toolkit)

Scikit-learn

**Setup and Installation**

**Clone the repository:**

git clone https://github.com/karthik1438/Movie-Recommendation-System.git

cd Movie-Recommendation-System

**Create a virtual environment (recommended):**

python -m venv venv
Activate the virtual environment:

.\venv\Scripts\activate

**Install the required libraries:**

pip install numpy pandas nltk scikit-learn
Note: You might need to download NLTK data. After installing NLTK, run python -c "import nltk; nltk.download('all')" in your Python environment.

Usage
Place the dataset: Ensure the movies_dataset.csv file is in the same directory as Code.ipynb.

**Run the Jupyter Notebook:**

jupyter notebook Code.ipynb

Follow the cells in the notebook to:

Load and preprocess the data.

Perform stemming on the movie tags.

Create text vectors using CountVectorizer.

Calculate cosine similarity between movie vectors.

Use the recommend() function to get movie recommendations.

Example Usage in the Notebook:
In the last cell of the notebook, you'll find an input() prompt. Enter a movie title, and the system will provide recommendations.

recommend(input("Enter movie title: "))

<img width="1471" height="349" alt="image" src="https://github.com/user-attachments/assets/8008ced5-bd73-4de4-a6ca-0c973745faca" />

Project Structure
Movie-Recommendation-System/

├── Code.ipynb              # Jupyter Notebook containing the main project code

├── movies_dataset.csv      # The dataset used for movie recommendations

└── README.md               # This README file
