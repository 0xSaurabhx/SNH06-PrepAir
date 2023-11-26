# LinkedIn Analytics Dashboard

This is a Streamlit dashboard for analyzing LinkedIn profile and post data. It allows extracting key metrics from your own or competitor profiles to benchmark performance.

## Features

- Profile metrics dashboard
  - Shows summary stats for your profile: likes, appreciations, impressions etc. 
  - Top posts ranked by engagement 
  - Historical trends over time
- Post analysis 
  - Sentiment analysis of comments using AI
  - Visualizations of reactions and engagement  
- Competitor benchmarking
  - Extract comments, profiles from competitor pages 
  - Analysis to compare performance vs competitors

## Getting Started

### Prerequisites

You need to install:

- Python 3.7+ 
- Streamlit 
- Pandas, Numpy etc for data analysis
- Selenium for web scraping LinkedIn pages

Register for these APIs:

- LinkedIn data API to extract profile/post metrics
- AI text analysis API for sentiment analysis 

### Installation

```
git clone https://github.com/<username>/linkedin-analytics.git
cd linkedin-analytics
pip install -r requirements.txt
```

### Configuration

Add RapidAPI keys and other credentials to a `.env` file:

```
LINKEDIN_API_KEY=xxx
AI_API_TOKEN=yyy 
```

### Run Locally

```bash
streamlit run app.py
```

It will open a browser window at `localhost:8501` with the dashboard.

## Usage

The sidebar menu allows choosing different analysis options:

**My Info:** Enter your LinkedIn URL. Fetches profile metrics and top posts ranked by engagement.

**Post Analysis:** Enter any LinkedIn post URL. Fetches comments and analyzes sentiment.

**Competitor Analysis:** Enter competitor profile username and login creds. Extracts comments, profiles and analyzes to benchmark vs your profile. 

## Roadmap

Some potential features:

- Automated post scheduling 
- Job search integration
- Lead generation tracking
- Multiple profile comparison

## Documentation

The key Python files are:

**app.py:** Main Streamlit app dashboard which also has below functions:
Functions to extract LinkedIn data  
Functions to analyze metrics, run AI analysis   
Functions to plot charts, graphs  

## License

This project is open source and available under the [MIT License](LICENSE).

Let me know if you would like any changes in this draft README!
