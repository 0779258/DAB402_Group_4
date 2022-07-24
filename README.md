# Proposing mental-health intervention strategies based on client intake form data

<p align="center">
  <img width="700" src="https://user-images.githubusercontent.com/106260176/180633483-2d705555-d701-4f7a-baf4-9bd4cab390dd.jpg" >
</p>

## Overview of the Problem
Mental diseases are illnesses that affect emotion, thought, and behaviors (or a combination of these). Distress and/or difficulty dealing with daily tasks at work, in the family, or in social situations are symptoms of mental diseases.
Depression, suicidal thoughts, bipolar disorder, autism spectrum disorder (ASD), anxiety disorder, schizophrenia, and other mental diseases can all have a severe impact on an individual's physical health and well-being.​
Many people who suffer from mental illnesses are hesitant to share it. However, mental illness is not a cause for shame! Like heart disease or diabetes, it is a medical issue. Additionally, mental health issues are treatable. As our knowledge of the human brain's working continues to grow, people can successfully manage their mental health disorders with the use of medications.

Causes are : Anything can trigger the mental trauma

Solutions : See a Certified Mental Health Professional immediately

## Background
Adults with depression and/or anxiety are significantly more likely to smoke, to be obese, to be physically inactive, to binge drink, and to drink more heavily than those who do not display any symptoms of depression and/or anxiety.
We can collect text data for mental health from a variety of sources, including social media posts, screening surveys, descriptive writing, interviews, and electronic health records (EHRs).  
At the same time, the datasets differ in terms of the types of illnesses they focus on and the languages they use for different detection tasks. Previous studies has shown that text can detect mental problems, but those studies focused on screening for a single specific disorder rather than multiple disorders at the same time.

## Research Objective
- Based on the problem statement, the following questions are posed: 
- To begin with, the background research helped in understanding a lot of past work that has contributed to the technologies and methodologies used to predict mental health using various machine learning techniques.
1. What are the benefits and risks of delivering mental health care through technology instead of face-to-face and what impact does the removal of face-to-face human interaction have?
2. Which machine learning techniques work the best to detect mental health in a patients from their intake form and how can we validate the accuracy of such prediction?

## Data Source Overview
- For this project,data was taken from patients by using google Mental Health Survey form. We initially designed an Intake Form which was not yet designed for the company up to the industry standards. We have collected data of 25 individuals till this time. It includes around 35 questions from which there are 5 more important fields for us on which we are focusing at this moment for the analysis purpose.
he main focus, we are giving is on "symptoms" of the patient intake form.
- The Mental Health Survey form can be found at this link: https://forms.gle/C3eaVanLpnWAchey9.

## Methods
- To begin, we used intake form text data as input. We already know that text data contain not only text but also noisy data such as symbols, emojis, numbers, and stop words.
 Furthermore, not all alphabets follow the same format, such as lowercase or uppercase. So, before we design any kind of model, we need to preprocess our data and remove all noise data, which is why we created a data cleaning function. It is converting all text characters into lowercase characters, removing punctuation and digits, stopping words and other common, unnecessary elements, and tokenizing all words. Tokenization requires extracting each unique word and then generating a dictionary in which each unique word is allocated an index.
- The following are the steps involved at each stage represented in given figure:
  1.  Data Extraction
  2.  Data Filtering from text data of clients
  3.  Data Cleaning:     Removal of Punctuation Mark, Removal of HTML Tags, Removal of Stop Words, Removal of URL, Extracting Sentiments of emojis
  4.  Sentiment Analysis
  5.  Word Cloud
  6.  Train/create models
  7.  Evaluate models 
- Here, we used SVC,Linear SVC, RandomForest and DecisionTree Machine learning models for our project. Following table shows the accuracy of our train and test data:

<p align="center">
  <img width="700" src="https://user-images.githubusercontent.com/106260176/180634480-12057a8a-0e62-4f9f-aa57-6cae4ed43903.png" >
</p>

## Results

<p>
  <img width="400" src="https://user-images.githubusercontent.com/106260176/180634639-c46abaa2-083d-4aae-8394-ca7e0317b9f9.png" >
  <img width="500" src="https://user-images.githubusercontent.com/106260176/180634679-f73b8d5f-9ff1-4695-b265-f7c9324e527b.png" >
</p>

## Future Work
- In future we can develop an API which can directly get input from the intake form data and can directly predict the diseases. 
- We can enhance this project with Audio and Video as well Speech to Text can also be added so that one doesn’t need to fill out the whole form and we can get the voice modulated answers. 

## References
- What is Mental Illness? (2016, August 14). Https://Psychiatry.Org/Patients-Families/What-Is-Mental-Illness#:~:text=Mental%20illnesses%20are%20health%20conditions,Nothing%20to%20be%20ashamed%20of. https://psychiatry.org/patients-families/what-is-mental-illness#:%7E:text=Mental%20illnesses%20are%20health%20conditions,nothing%20to%20be%20ashamed%20of.
- https://www.ukessays.com/essays/social-work/mental-health-policy-thesis-statement-social-work-essay.php























