# Machine Translation-Enabled Sentiment Analysis Across Multiple Languages

## Data Collection

![Example Image 1](https://github.com/sushantmenon1/Machine-Translation-Enabled-Sentiment-Analysis-Across-Multiple-Languages/assets/74258021/7eb76474-78b8-409b-8613-eaff8a861165) &rarr; ![Example Image 2](https://github.com/sushantmenon1/Machine-Translation-Enabled-Sentiment-Analysis-Across-Multiple-Languages/assets/74258021/733a53b8-ebb0-4c37-b20e-6852fbf34fb8)


The data for the project was sourced from Kaggle, a platform for data scientists and machine learning engineers to share and discover datasets. Specifically, the dataset used was the Amazon Alexa Reviews dataset, which consists of customer reviews of the Amazon Alexa device. The dataset was collected through web scraping, which involves using software to automatically extract data from websites. The code used to scrape the data is not provided, but the dataset is publicly available on Kaggle and can be accessed and verified by anyone. It is possible to re-collect the data, but it would require replicating the web scraping process used to obtain it. It is worth noting that the data is proprietary, as it belongs to Amazon, but it has been made publicly available for research purposes.

Kaggle Link: [Amazon Alexa Reviews Dataset](https://www.kaggle.com/datasets/sid321axn/amazon-alexa-reviews)

## Data Management
Data pre-processing and cleaning were performed to ensure that the data was ready for analysis. Several techniques were used, including removing duplicate entries, removing irrelevant columns, and converting the data into a suitable format. These steps aided in improving the data's quality and eliminating any inconsistencies that could have influenced the analysis's results.

There was no recoding of variables after the data was collected. To ensure the accuracy of the results, the data was analyzed in its original form. Furthermore, no other data was merged with the existing data, and no data was manually manipulated after it was collected. This method ensured that the data analysis was done objectively and thoroughly. Overall, the data cleaning and management process was methodical and efficient. The data was handled with care, and all steps were documented to ensure the analysis's integrity. To avoid bias in the results, the data was analyzed in its original form with no manual manipulation.

Because the text data can be in any language, the first step in the process is to change the text data to English. We will be using the Google Translate API to perform this Machine Translation task. After this process, we can start the cleaning part of the project.

We have designed a cleaning function in which we have used some components of the popular Natural Language Processing Library nltk (Natural Language Toolkit). We will be using techniques such as Stop Word Removal and Lemmatization. We have also used the library `re` to remove any unwanted characters in our text data.

## Text Analysis Steps

1. **Optical Character Recognition (OCR)**: In the first step, we read the text from the image. This step involves the use of an optical character recognition (OCR) tool like `pytesseract` to extract the text from the image. Once we have the text, we can move on to the next step. Please note that this is part of phase 3 and will only be focused upon if time permits.

2. **Language Translation**: The second step involves converting the language of the text to English using the Google Translate API. This step is important when dealing with text that is written in languages other than English. By converting the text to English, we can ensure that our text analysis models work effectively.

3. **Sentiment Analysis**: In the third step, we train and test our model or use a pre-trained sentiment classifier like Vader. The goal of this step is to analyze the sentiment of the text. Sentiment analysis involves classifying the text into positive, negative, or neutral categories. By analyzing the sentiment of the text, we can gain insights into the feelings and opinions of the text's author.

4. **Predicting Sentiment for Streaming Data**: Once we have our model or sentiment classifier, we can move on to the fourth step, which involves predicting sentiment for streaming data. Streaming data refers to data that is generated in real-time, such as social media posts or news articles. By predicting sentiment for streaming data, we can keep track of the changing opinions and feelings of the public on different topics.

## Pytesseract
Pytesseract is a Python library that provides an interface for interacting with Tesseract OCR (Optical Character Recognition) engine. It allows developers to extract text from images or scanned documents by utilizing Tesseract's powerful text recognition capabilities. With Pytesseract, you can easily incorporate OCR functionality into your Python projects, enabling tasks such as automated data extraction, text recognition, and image-to-text conversion. It supports a wide range of image formats and provides flexibility in configuring OCR parameters for better accuracy. Pytesseract simplifies the integration of OCR technology into Python applications, making it a valuable tool for various applications like document processing, image analysis, and automated data extraction from images.

pytesseract 0.3.10 :- `pip install pytesseract`
