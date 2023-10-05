# Web Data Sentiment Analyzer

## Overview

This project involves the extraction and analysis of textual data from a list of URLs. The goal is to gather information, calculate various text analysis metrics, and generate insights from the extracted content. The project includes web scraping, sentiment analysis, readability assessment, and the calculation of linguistic features.

## Project Components

### 1. Data Extraction

The project begins by reading a list of URLs from an Excel file ('Input.xlsx') using the Pandas library. The URLs are then visited, and data is extracted using the `requests` library and web scraping techniques. The extracted data includes titles, content, and the HTML structure of the web pages.

### 2. Sentiment Analysis

Sentiment analysis is performed to determine the overall sentiment of the extracted text. The analysis involves:

- Calculating positive and negative sentiment scores for each text entry.
- Computing a polarity score to gauge overall sentiment.
- Estimating subjectivity scores to measure the subjectivity of the text.

### 3. Readability Assessment

The readability of the text is assessed using the Gunning Fog Index, which estimates the readability level of the text based on sentence length and the percentage of complex words. The project calculates:

- Gunning Fog Index scores for each text entry.
- Average words per sentence to gauge sentence length.
- Counts of complex words.
- Syllable counts for estimating word complexity.
- Counts of personal pronouns.
- Average word lengths.

## Final Data Export

The processed data is compiled into a final dataset ('final_data') that includes a wide range of text analysis metrics. The selected columns are saved to a CSV file ('output.csv') for further analysis or reporting.

## Usage

You can use this project to:

- Analyze the sentiment and subjectivity of textual content.
- Assess the readability of text using the Gunning Fog Index.
- Extract various linguistic features for text analysis.
- Generate insights from web content.

## Dependencies

This project relies on several Python libraries, including:

- Pandas for data manipulation.
- BeautifulSoup for web scraping.
- NLTK (Natural Language Toolkit) for text analysis.
- Regular expressions for pattern matching.

## Installation and Usage

To use this project, follow these steps:

1. Clone the repository to your local machine.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Place your list of URLs in an Excel file named 'Input.xlsx.'
4. Run the provided Python script to perform data extraction and analysis.
5. Review and analyze the output data in 'output.csv.'

## Credits

- [Pandas](https://pandas.pydata.org/)
- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)
- [NLTK](https://www.nltk.org/)

## Acknowledgments

Special thanks to the open-source community and the developers of the libraries used in this project for their contributions.
