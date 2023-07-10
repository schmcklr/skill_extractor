# Job Skills Analysis [![Under Development](https://img.shields.io/badge/status-Under%20Development-yellow.svg?color=yellow)](https://img.shields.io) [![Google Colab Notebook](https://img.shields.io/badge/Google%20Colab-Open-orange?logo=google-colab)](https://colab.research.google.com/)

The objective of this project is to analyze job descriptions in order to identify the skills required for these positions. The goal is to gain an understanding of how skill requirements have evolved over time.

## Methodology
The project uses job listings data provided by the platform JobTeaser. The project includes translation, natural language processing, and topic modeling techniques to extract relevant information from the job descriptions.

## Implementation
The project is implemented in Python and makes use of various libraries such as pandas, nltk, re, requests, numpy, gensim, odfpy, IPython, BeautifulSoup, googletrans, translatepy, langdetect, pyldavis, LdaOverTime and matplotlib.

## Project Structure

The project is divided into three parts:

- **Part 1: General Preprocessing and Translation**

  Designed to filter out duplicate job postings, translate non-English job postings into English language, and perform initial general preprocessing. The results will be outputted in an Excel file, which can be used for further analysis.

- **Part 2: Skill Section Extraction and Preprocessing**

  Systematically extracts the qualification section from English job ads by scouring the HTML source code. It identifies key phrases and specific patterns, derived from the analysis of over 1500 job ads. The extracted qualifications, along with the remaining job ad data, are compiled in a data frame and exported to an Excel file for further analysis. Ads where the qualification section couldn't be extracted are automatically excluded from the export.

- **Part 3: Skill Analysis**

  Offers a variety of features designed to track and analyze the progression of desired job qualifications over time. The program should be executed in Google Colab with GPU acceleration enabled. There are two implemented options for this:

  1. Static LDA Topic Modeling & Skill-Count Analysis
  2. Dynamic LDA Topic Modeling

## Getting Started
- Please open the notebook in Google Colab and execute the cells sequentially.
