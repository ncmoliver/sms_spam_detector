# Spam Detector

# Overview

This "Spam or Not Spam" classifier processes text messages to determine if they contain spam content. It uses a natural language processing (NLP) pipeline that first transforms text data using TF-IDF (Term Frequency-Inverse Document Frequency) to represent word importance and then classifies the text with a linear SVM classifier. The model is then integrated into a gradio front-end for user consumption.

## Features

**Text Processing with TF-IDF:** The text messages are transformed into numerical vectors using TF-IDF, highlighting the importance of certain words.
**Classification with Linear SVM:** The transformed data is classified as "Spam" or "Not Spam" using a linear SVM classifier, chosen for its effectiveness with high-dimensional data.
**Gradio Front-End:** The model is accessible via a web interface created with Gradio, allowing users to input their own messages and get immediate feedback on whether they are spam.

## Getting Started

#### Prerequisite

- Python 3.7 or higher
- Required Libraries (listed in requirements.txt)

#### Installation

1. Clone the repository:
   `git clone https://github.com/ncmoliver/sms_spam_detector.git`
2. Install the dependencies:
   `pip install requirements.txt`
3. Run the file & enjoy! `gradio_sms_text_classification.ipynb`

#### Usage

Enter a
