# Analyzing U.S. Presidential Inaugural Addresses

This project focuses on analyzing the U.S. Presidential inaugural addresses using Natural Language Processing (NLP) techniques. The primary goal is to extract and analyze adjectives used in these speeches, providing insights into how Presidents have described various aspects of America over time.

## Project Overview

### Objectives

1. **Data Collection**:
   - Retrieve the text of U.S. Presidential inaugural addresses from the NLTK inaugural corpus.
   - Load and preprocess the text data for further analysis.

2. **Adjective Analysis**:
   - Identify the most common adjectives used in each inaugural address.
   - Analyze trends in the use of specific adjectives across different presidencies.

3. **Adjective Trends Over Time**:
   - Track the frequency of key adjectives, such as "great," "other," and "own," over time.
   - Visualize these trends to understand how Presidential rhetoric has evolved.

4. **Descriptive Analysis of America**:
   - Focus on how Presidents have described "America" in their speeches.
   - Extract and analyze the adjectives used specifically to describe "America."

## Data Sources

- **NLTK Inaugural Corpus**: The project utilizes the inaugural corpus from the NLTK library, which contains the full text of U.S. Presidential inaugural addresses from 1789 to the present.

## Key Steps and Functions

### 1. Data Retrieval

- The inaugural addresses are retrieved using the `inaugural.fileids()` function from the NLTK corpus.
- Each speech is tokenized and stored in a list for further processing.

### 2. Most Common Adjectives

- **Function**: `most_common_adjs(text)`
  - This function extracts all adjectives from a given text and identifies the most common one.
  - The output is a tuple containing the adjective and its frequency.

- **Analysis**:
  - The function is applied to each inaugural address to create a list of the most common adjectives.
  - A DataFrame is created to store these adjectives along with their frequencies.

### 3. Adjective Trends Over Time

- **Tracking Key Adjectives**:
  - Adjectives such as "great," "other," and "own" are tracked across different Presidential addresses.
  - A DataFrame is constructed to hold the counts of these adjectives for each President and year.

- **Visualization**:
  - A bar plot is created to visualize the frequency of these adjectives over time, highlighting the most common descriptors in Presidential rhetoric.

### 4. Describing America

- **Function**: `describe_america(text)`
  - This function focuses on adjectives that directly describe the word "America" within the text.
  - The output is a list of adjectives used to describe "America" in the inaugural addresses.

- **Analysis**:
  - The function is applied to each address to compile a list of adjectives that have been used to describe America.

## Results

### Most Common Adjectives in Inaugural Addresses

- Adjectives like "great," "other," and "own" have been frequently used across multiple Presidential speeches.
- The most frequently used adjective in the corpus is "great," appearing 332 times.

### Trends in Adjective Use

- The frequency of specific adjectives varies significantly across different Presidential terms.
- The term "new" was notably prominent in President Clinton’s 1997 address, reflecting the forward-looking nature of the speech.

### Descriptions of America

- Descriptive terms such as "productive," "strong," and "rich" have been used by Presidents to describe America.
- These adjectives reflect the prevailing themes and priorities of the respective administrations.

## Conclusion

This project provides insights into how U.S. Presidents have used language, particularly adjectives, to convey their messages and describe the nation. By analyzing these patterns, we can gain a better understanding of the evolving rhetoric in American political discourse. Further exploration could include analyzing other parts of speech or comparing the inaugural addresses with other types of Presidential speeches.

## Requirements

- Python 3.x
- NLTK
- SpaCy
- Pandas
- Matplotlib (for visualization)

## Installation

To install the required libraries, use the following pip commands:

```bash
pip install nltk spacy pandas matplotlib
python -m spacy download en_core_web_sm
```

## How to Run

1. Ensure all required libraries are installed.
2. Download the NLTK inaugural corpus using `nltk.download("inaugural")`.
3. Run the script to perform the analysis.

The analysis will output the most common adjectives, track their usage over time, and identify adjectives used to describe "America" in Presidential inaugural addresses.
