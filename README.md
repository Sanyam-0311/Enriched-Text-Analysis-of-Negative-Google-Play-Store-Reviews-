# Enriched-Text-Analysis-of-Negative-Google-Play-Store-Reviews-

This project involves scraping, preprocessing, and analyzing negative reviews (1-star and 2-star) from the Google Play Store for a specific app. The goal is to extract meaningful insights using Natural Language Processing (NLP) techniques, cluster the reviews, and visualize the results.

## Installation

To run this project, you need to have Python installed. You can install the required packages using `pip`:

## Project Overview

This project is aimed at extracting and analyzing negative reviews from the Google Play Store to identify common issues faced by users. The analysis includes keyword extraction, clustering, and various visualizations.

## Data Collection

Reviews are fetched using the `google-play-scraper` library. The script extracts all reviews written in English and filters them for 1-star and 2-star ratings.

## Preprocessing

Basic preprocessing steps include:
- Removing non-alphabetic characters and converting text to lowercase.
- Lemmatizing the text to reduce words to their base forms.
- Removing stopwords to focus on meaningful terms.

## Keyword Extraction

The `summa` library is used to extract important keywords from the processed reviews. These keywords help in summarizing the content of the reviews.

## Clustering

KMeans clustering is applied to group similar reviews together. The reviews are vectorized using TF-IDF before being clustered into a specified number of groups.

## Visualization

The following visualizations are included:
- **Heatmap**: Displays the frequency of key terms across different clusters.
- **Scatter Plot**: Visualizes the clusters in a reduced 2D space using PCA.
- **Word Clouds**: Generates word clouds for each cluster to show common terms.

## Results

The processed reviews, along with their corresponding clusters and keywords, are saved in an Excel file (`Output_Data_Enriched.xlsx`). This file contains the enriched data that can be used for further analysis.

## Output

The results of the analysis are saved in `Output_Data_Enriched.xlsx`. This file contains:
- Original reviews and ratings.
- Cleaned and processed reviews.
- Extracted keywords.
- Cluster labels assigned to each review.
- PCA components for visualization.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you would like to contribute to this project.
