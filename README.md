# Citizenship-Data-Extraction-using-Tesseract
Just created a SIMPLE OCR which helps to Digitize your Citizenship [ back side of Nepali citizenship as it is in English ]. I used Tesseract-OCR to build this. 

## What I basically did?

### 1. Preprocess the data [ converting image to grayscale, blurring image and then adding threshold ]
- We need to grayscale as most OCR use black and white image
- I added thershold of 50 to convert any pixel below 50 to 0 and other to 255. It helps to capture word cleary

### 2. Sending the image to Tesseract OCR
- Using filters to separate the characters from the background
- Apply contour detection to recognize the filtered characters
- Use mage classification to identify the characters

### 3. Information Extraction
- OCR gives the raw text. We have to extract useful information from there.
- I used regex and other slicing for extracting information that I need.
