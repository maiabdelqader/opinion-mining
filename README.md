# Opinion Mining in Product Reviews

The Opinion Mining Jupyter notebook provides a comprehensive approach to analyzing sentiments expressed in product reviews. It combines Natural Language Processing (NLP), data mining, and computational linguistics to categorize opinions and understand emotional tones in text. This tool is invaluable for businesses and researchers who aim to glean insights from customer feedback.

## Data Structure and Content

#### Overview of Data
The data used in this notebook consists of annotated customer reviews of three products: Computer, Wireless Router, and Speaker. These reviews are sourced from amazon.com and are utilized for opinion mining and sentiment analysis.

#### Data Format and Annotation
The dataset is organized into multiple files, each containing reviews for a different product. Each product has a text file (e.g., Computer.txt). The reviews are stored in a standardized format, as detailed below, ensuring uniformity and consistency for analysis:

- **Review Content**: The reviews are annotated with product features/aspects and their associated sentiments.
- **Symbols in Reviews**:
  - `[t]`: Indicates the title of the review. Each `[t]` tag starts a review.
  - `xxxx[+|-n]`: Represents a product feature (`xxxx`). `[+n]` indicates a positive opinion with `n` being the opinion strength (1 to 3). `[-n]` indicates a negative opinion.
  - `##`: Marks the start of each sentence in the text file.
  - `[a]`, `[v]`: Represent implicit features implied by adjectives or verbs.
  - `[u]`: Feature not appeared in the sentence.
  - `[p]`: Feature not appeared in the sentence, requiring pronoun resolution.
  - `[s]`: Suggestion or recommendation.
  - `[cc]`: Comparison with a competing product from a different brand.
  - `[cs]`: Comparison with a competing product from the same brand.

## Usage

#### Running the Opinion Mining Notebook

To run the notebook, you need a Jupyter environment. You can use either Jupyter Notebook or JupyterLab. Open the `opinion-mining.ipynb` file in your Jupyter environment to start.

```shell
jupyter notebook opinion-mining.ipynb
```

The notebook is structured into various sections, including data parsing, preprocessing, feature extraction, sentiment analysis, and evaluation. Follow the cells in sequence for a step-by-step analysis. Users can modify parameters and methods according to their dataset and analysis requirements.

#### Key Components of the Notebook

This section outlines the key components and methodologies used in the notebook, such as data preprocessing, feature extraction techniques, sentiment analysis using VADER and Naive Bayes, and various evaluation metrics.

## Features

- Detailed analysis of product reviews using NLP and machine learning techniques.
- Parsing and preprocessing of review data.
- Extraction of key product features from text.
- Sentiment analysis with SentimentIntensityAnalyzer from VADER and Naive Bayes.
- Evaluation of feature extraction and sentiment analysis using precision and recall metrics.

## Dependencies

The notebook requires the following dependencies:

- Python 3.x
- Natural Language Toolkit (nltk)
- Pandas
- NumPy
- scikit-learn
- vaderSentiment

## Installation

1. Clone the repository or download the notebook file.

2. Install the required Python libraries:

   ```shell
   pip install nltk pandas numpy scikit-learn vaderSentiment
   ```

3. Open the notebook in a Jupyter environment.

## Contributing

Contributions to the Opinion Mining project are encouraged. If you have suggestions or improvements, please open an issue or submit a pull request on GitHub.