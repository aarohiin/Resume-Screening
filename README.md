# Resume Screening Application

## Description

This is a Streamlit web application that performs resume screening using machine learning. It classifies resumes into different job categories based on their content.

## Features

- Upload resume files (TXT or PDF)
- Clean and preprocess resume text
- Classify resumes into 25 different job categories
- Display the predicted job category

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/resume-screening-app.git
   cd resume-screening-app
   ```

2. Install the required packages:
   ```
   pip install streamlit pickle-mixin nltk scikit-learn
   ```

3. Download NLTK data:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   ```

## Usage

1. Ensure you have the trained models (`clf.pkl` and `tfidf.pkl`) in the correct directory.

2. Run the Streamlit app:
   ```
   streamlit run app.py
   ```

3. Open your web browser and go to `http://localhost:8501`.

4. Upload a resume file (TXT or PDF) and see the predicted job category.

## Model Information

The application uses two pre-trained models:
- A classifier model (`clf.pkl`)
- A TF-IDF vectorizer (`tfidf.pkl`)

These models should be placed in the same directory as the script.

## File Structure

```
resume-screening-app/
│
├── app.py
├── clf.pkl
├── tfidf.pkl
└── README.md
```

## Dependencies

- streamlit
- pickle
- re
- nltk
- scikit-learn (implied by the use of TF-IDF and classifier)

## Author

Aarohi Mritunjay Singh

