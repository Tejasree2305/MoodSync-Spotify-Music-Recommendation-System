# MoodSync - Spotify Music Recommendation System

## Project Overview

MoodSync is a Python-based music recommendation project
developed using Spotify audio features.

The project explores song characteristics, classifies
songs into mood categories, and recommends music based
on mood or audio-feature similarity.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Google Colab

## Dataset

Original dataset: 114,000 songs

After removing rows with missing required values:
113,999 songs

After removing duplicate track IDs:
89,740 unique tracks

## Project Workflow

1. Data loading and exploration
2. Data cleaning and duplicate removal
3. Exploratory data analysis
4. Mood classification
5. Audio-feature analysis
6. Mood-based song exploration
7. Content-based recommendations
8. Recommendation evaluation
9. Input validation and automated testing

## Mood Classification

Songs are classified using energy and valence.

Mood categories:

- Happy / Energetic
- Happy / Calm
- Sad / Calm
- Intense / Low-Valence

## Recommendation Methods

### Mood-Based Recommendations

Songs are filtered by mood and ranked by popularity.

### Content-Based Recommendations

The system uses seven audio features:

- Danceability
- Energy
- Valence
- Acousticness
- Instrumentalness
- Speechiness
- Liveness

Cosine similarity is calculated using NumPy to
identify songs with similar audio characteristics.

## Evaluation Results

Example input song: Comedy

- Recommendations evaluated: 5
- Average cosine similarity: 0.9974
- Minimum cosine similarity: 0.9972
- Maximum cosine similarity: 0.9978
- Unique mood categories: 2
- Mood diversity ratio: 0.4000
- Average pairwise Euclidean distance: 0.1991
- Spearman rank correlation: 0.3000

These are descriptive evaluation metrics.
They do not establish listener satisfaction
or recommendation accuracy.

## Automated Testing

Eight input-validation tests were performed.

- Total tests: 8
- Passed tests: 8
- Failed tests: 0
- Pass rate: 100%

The tests cover valid and invalid song titles
and recommendation-count inputs.

## Project Results

Evaluation reports are available in:

results/moodsync_evaluation_summary.csv

results/moodsync_automated_test_report.csv

## Limitations

- Recommendations use audio-feature similarity.
- Listener preferences were not collected.
- The evaluation does not measure user satisfaction.
- Songs with identical titles may be ambiguous.
- The system has not been deployed as a web application.

## Future Improvements

- Add artist-based song selection
- Improve recommendation diversity
- Add a user-friendly interface
- Evaluate recommendations using listener feedback

## Project Purpose

This project demonstrates practical skills in
data cleaning, exploratory data analysis,
feature engineering, recommendation algorithms,
evaluation, and Python programming.
