# Lizmotors mobility Internship coding assignment 2024

A sample RAG implementation as instructed in the problem statement.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.

```bash
pip install -r requirements.txt
```

## Usage

```python
python submission.py
```

## Steps Involved

1. I started with the search query generation, since I don’t have a GPU enabled 	machine I used openai api to generate search queries based on the user query first the gpt generates 5 search queries for the user query.
2. As second step I used duckduckgo search api to get top 2 most relevant links for each subquery (search query)
3. Then developed a web scraping tool to scrape text from the web pages using beautiful soup.
4. As the scraped data was too big to be fitted in single context window of general LLMs I decided to divide the data into small chunks and summarize it using T5-small model on local machine.
5. Then I passed the summarized data to openai api with the subquery to generate a small report using the summarized data and query.
6. Collected such small reports to answer the large user query with multiple subquestions.

## Report file

new_report.docx is contains the automatically generated content from the python script submission.py you can refer the ipynb file to know about the development environment.
## Contact

[Pranav Chougule](chougulepranav@yahoo.com)
