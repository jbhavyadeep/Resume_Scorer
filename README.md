# ResumeScorer (AI Powered)

## Table of Contents
- [Introduction](#introduction)
- [Functionalities](#functionalities)
- [Launch](#launch)
- [Screenshots](#screenshots)
- [Technologies](#technologies)

## Introduction
The Resume Scorer project seeks to create a platform where users can upload their resumes and job descriptions and receive a similarity score that indicates how well the resume matches the job requirements. Furthermore, the system provides optimisation ideas to help the CV correspond with the job description. The platform makes it easier for job seekers and recruiters to apply for jobs by using text recognition and similarity scoring algorithms.

## Functionalities
- **Login and Registration:** Users authenticate using AWS Cognito for secure access to premium features and recruiters' services.
- **Resume and Job Description Upload:** Resumes and job descriptions are uploaded to an AWS S3 bucket for storage and retrieval.
- **Text Recognition:** AWS Textract service is utilized to extract text from uploaded documents.
- **Contact Information Extraction:** The first 250 characters of documents are passed to AWS Comprehend service for contact information extraction, benefiting recruiters.
- **Similarity Scoring:** The system calculates a similarity score between uploaded resumes and job descriptions.
- **Resume Optimization Suggestions:** Suggestions are provided to users for incorporating missing keywords to enhance their resume's alignment with job descriptions.


## Launch

### Setup
1. pip install -r requirements.txt
2. Config AWS: $ aws configure
3. To Run Backend
	
```bash
$ cd Capabilities
$ chalice local --port 3001
```

4. To Run FrontEnd
	
```bash
$ cd Website/
$ python3 -m http.server 8080
```

Then go to localhost:8080.

## Screenshots
- **HomePage**
  ![HomePage](/Website/images/HomePage.jpeg)

- **Login & Register Page**
  ![Login & Register Page](/Website/images/LogInPage.jpeg)

- **LandingPage**
  ![LandingPage](/Website/images/LandingPage.jpeg)  

- **Report**
  ![Report](/Website/images/ScoreDisplay.jpeg)
  

## Technologies

- Python
- AWS (Amazon Web Services) - utilized services include:
  - Amazon Cognito
  - Amazon S3 (Simple Storage Service)
  - Amazon DynamoDB
  - Amazon Textract
  - Amazon Comprehend
- Chalice - Python serverless microframework for AWS Lambda
- NLTK (Natural Language Toolkit) - Python library for natural language processing
- scikit-learn - Python library for machine learning tasks
- Bootstrap - front-end framework for building responsive and mobile-first websites
- Font Awesome - icon toolkit used for icons in the user interface
- JavaScript - programming language for client-side scripting
- HTML - markup language for creating web pages
- CSS - style sheet language for styling HTML elements
- Flask - web framework for Python (imported from Chalice)
- Requests - Python HTTP library for making requests
- Base64 - encoding and decoding library
- Boto3 - AWS SDK for Python
- datetime - module for manipulating dates and times in Python
- os - module for interacting with the operating system
- re (Regular Expressions) - Python module for working with regular expressions
- Counter - Python module for counting hashable objects
- time - module for working with time in Python
- CORS (Cross-Origin Resource Sharing) - mechanism to allow or restrict requested resources on a web server
- Git - version control system
- GitHub - platform for hosting and sharing Git repositories


