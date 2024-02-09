## Web Scraping and Text Analysis for Sentiment Analysis

### Overview:
This project involves web scraping articles from provided URLs, performing text analysis, and computing various metrics including sentiment analysis. The analysis is conducted using Python with libraries such as BeautifulSoup, pandas, nltk, and requests.

### Workflow:
1. **Data Collection:**
   - URLs of articles are provided in a CSV file.
   - Using pandas, the CSV file is loaded to fetch the URL data.

2. **Text Preprocessing:**
   - The article text is scraped from each URL using BeautifulSoup.
   - Preprocessing steps include:
     - Removing HTML tags and unnecessary whitespaces.
     - Tokenization of text into words.
     - Removal of punctuation and stop words specific to various categories like auditor names, currencies, dates, etc.

3. **Sentiment Analysis:**
   - A master dictionary of positive and negative words is imported.
   - Sentiment scores are computed based on the frequency of positive and negative words found in the article text.
   - Polarity and subjectivity scores are calculated based on the sentiment analysis results.

4. **Additional Text Metrics:**
   - Various text metrics are computed, including average sentence length, percentage of complex words, Fog Index, average number of words per sentence, syllables per word, personal pronouns count, and average word length.

5. **Output:**
   - The results are stored in a pandas DataFrame.
   - The DataFrame is exported to an Excel file for further analysis and reporting.

### Usage:
- Ensure the necessary Python libraries are installed.
- Modify paths to input files (CSV containing URLs) and stop word lists as per your directory structure.
- Run the script to perform web scraping and text analysis.
- Check the generated Excel file (`Answer.xlsx`) for the analyzed results.

### Dependencies:
- pandas
- requests
- BeautifulSoup
- numpy
- nltk
