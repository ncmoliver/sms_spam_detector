# SMS Text Message Spam Detector

![Spam detector logo, heading and electrical background image](spam_log.png)

# Overview

This "Spam or Not Spam" classifier processes text messages to determine if they contain spam content. It uses a natural language processing (NLP) pipeline that first transforms text data using TF-IDF (Term Frequency-Inverse Document Frequency) to represent word importance and then classifies the text with a linear SVM classifier. The model is then integrated into a gradio front-end for user consumption.

## Features

| Feature                            | Description                                                                                                                                                      |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Text Processing with TF-IDF**    | The text messages are transformed into numerical vectors using TF-IDF, highlighting the importance of certain words.                                             |
| **Classification with Linear SVM** | The transformed data is classified as "Spam" or "Not Spam" using a linear SVM classifier, chosen for its effectiveness with high-dimensional data.               |
| **Gradio Front-End**               | The model is accessible via a web interface created with Gradio, allowing users to input their own messages and get immediate feedback on whether they are spam. |

---

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

1. Type Your SMS Message  
   Enter a text message in the provided input box on the Gradio interface.

2. Classify  
   Click the "Submit" button.

3. Review The Results  
   The classifier will output either "Spam" or "Not Spam" based on the content in the message.

Example:

> Input (text message): "The drive home was super long today, too much traffic!"  
> Output: "Not Spam"

---

## Model Pipeline

**Data Preprocessing**  
Split dataset using train_test_split, into features (`X`) and target (`y`).

**Model Training**  
 A linear SVM model is trained on labeled text messages to distiguish between spam or not spam.

**User Interface**  
The model is deployed in a Gradio front-end for easy access.

---

# References

[Xpert Learning Assistant](https://bootcampspot.instructure.com/courses/6028/external_tools/313)
