# IDF Telegram Channel News Dataset

## Overview
This dataset is scraped from the IDF Telegram channel, the official “Israeli”  news update channel. It contains structured information extracted from news posts, which includes publication dates, textual content, and entities mentioned in the text. The dataset is ideal for natural language processing (NLP) tasks, entity recognition, and trend analysis.

## Features
The dataset includes the following features:

- Date: The publication date of the news post.
  - Type: Date
  - Format: YYYY-MM-DD
  
- Text: The textual content of the news post.
  - Type: String
  
- Location: Names of locations mentioned in the news text.
  - Type: String (List of locations)
  - Description: Extracted locations such as cities, countries, landmarks, etc.
  
- Person: Names of individuals mentioned in the news text.
  - Type: String (List of persons)
  - Description: Extracted names of people referenced in the news.
  
- Organization: Names of organizations mentioned in the news text.
  - Type: String (List of organizations)
  - Description: Extracted names of entities such as companies, government bodies, non-profits, etc.
  
- Siren: Indicator if the news text is about sirens being launched from or to a state.
  - Type: Boolean
  - Description: `1` if the news text mentions sirens being launched, `0` otherwise.
  
## Data Collection
The data was collected through web scraping techniques applied to the IDF Telegram channel. The scraping process was automated to ensure timely updates and coverage of all posts. Named entity recognition (NER) techniques were used to extract and categorize locations, persons, and organizations mentioned in the text.
Statistics


## Usage
This dataset can be used for various applications, including but not limited to:
- Natural Language Processing (NLP) tasks such as text classification, sentiment analysis, and entity recognition.
- Temporal analysis of news trends and events.
- Geographic analysis based on mentioned locations.
- Social network analysis of mentioned persons and organizations.
- Monitoring and alerting systems for siren-related news.

## Example
An example entry in the dataset is as follows:

```json
{
  "Date": "2024-05-20",
  "Text": "A major event happened in New York today. President John Doe announced a new policy. The United Nations headquarters were mentioned in the discussion. Sirens were heard as part of a drill.",
  "Location": ["New York"],
  "Person": ["John Doe"],
  "Organization": ["United Nations"],
  "Siren": 1
}
```

## Access
The dataset is available on GitHub at [repository link]. Users can clone the repository or download the dataset directly from the releases section.

## Contributions
Contributions to the dataset, such as improving the scraping methods, expanding the feature set, or enhancing data quality, are welcome. Please refer to the contribution guidelines in the repository.

## License
If you use IDF in your research, please cite the following paper:
bibtex @article{ }


For any questions or support, please open an issue in the GitHub repository.

