# GitHub Repository Recommendation System

A **GitHub Repository Recommendation System** that fetches user, repository, and README data from GitHub, preprocesses it, and provides repository recommendations based on similarity using **TF-IDF** and **cosine similarity**. This project integrates data extraction, NLP preprocessing, and recommendation algorithms.

---

## Table of Contents

- [Overview](#overview)  
- [Features](#features)  
- [Technologies](#technologies)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Project Structure](#project-structure)  
- [How it Works](#how-it-works)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Overview

This project extracts GitHub user details, repository information, and README content using the **GitHub API** and web scraping. The data is preprocessed with **NLP techniques** such as tokenization, lemmatization, and stopword removal. Using **TF-IDF** vectors and **cosine similarity**, the system recommends similar repositories to a user while avoiding repositories they already own or starred.

---

## Features

- Fetch GitHub user details, repositories, and README content.  
- Preprocess text data (names, descriptions, languages, readmes) using **NLTK** and **spaCy**.  
- Convert textual data to **TF-IDF vectors** for repository names, descriptions, languages, and README content.  
- Compute **cosine similarity** between repositories.  
- Recommend top repositories to a user excluding their own repositories.  
- Handle API rate limits efficiently.  

---

## Technologies

- **Python**  
- **MongoDB** (for storing GitHub data)  
- **Pandas** (data manipulation)  
- **NumPy & SciPy** (vector operations)  
- **NLTK & spaCy** (NLP preprocessing)  
- **Scikit-learn** (TF-IDF and cosine similarity)  
- **BeautifulSoup** (web scraping)  
- **GitHub API** (fetching repository and user data)  
- **Requests** (HTTP requests)

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/github-repo-recommendation.git
cd github-repo-recommendation
```
## Project Structure
github-repo-recommendation/
│
├── main.py                 
├── requirements.txt        
├── README.md                
├── .env                    
└── notebooks/     

## Contributing

Create a new branch: git checkout -b feature/your-feature

Commit your changes: git commit -m 'Add your feature'

Push to the branch: git push origin feature/your-feature

Create a Pull Request

## Result

Rank	Repository Name	Description	Languages	Similarity Score
1	awesome-python	A curated list of awesome Python frameworks, libs…	Python	0.89
2	machine-learning-algos	Collection of machine learning algorithms in Python	Python	0.87
3	deep-learning-tutorials	Tutorials for deep learning using PyTorch & Tensor…	Python	0.85
4	data-science-notebooks	Jupyter notebooks for data science projects	Python, Jupyter	0.83
5	nlp-resources	Resources for natural language processing projects	Python, NLP	0.82
