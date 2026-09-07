# Developer Salary Prediction

This project tries to predict developer salaries using data from the
Stack Overflow Developer Survey (2025). I used things like country,
years of experience, education, job type, and programming languages
to see how well I could predict someone's salary.

## What's in this project

- Cleaned up the raw survey data (there was a lot of missing data and
  some weird outliers to deal with)
- Made some charts to see how salary relates to country, experience,
  language, and job type
- Turned the text columns into numbers so a model could use them
- Trained two models (Linear Regression and Random Forest) and compared them
- Went with Random Forest as the final model

## Results

The model's accuracy wasn't amazing (R² around 0.24). I think that's
mostly because a lot of things that affect salary just aren't in this
survey - like the specific company, city, or how good someone is at
negotiating. I tried a couple of things to improve it (switching models,
log-transforming the salary) but got similar results either way.

## Built with

Python, pandas, scikit-learn, matplotlib, seaborn

## Running it

1. Clone the repo
2. Install the requirements: pip install pandas numpy scikit-learn matplotlib seaborn jupyter
3. Open 01_data_exploration.ipynb