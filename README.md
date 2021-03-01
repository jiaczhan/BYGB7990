# BYGB7990
#First README file that explains the functions of python files for Assignment 1
#The python file named "Twitter Crawling" which collect the twitter content including user account, publish date and content that related to certain topics
#First import the packages:
import re
import pandas as pd 
import numpy as np 
import matplotlib.pyplot as plt 
import seaborn as sns
import string
import nltk
import warnings 
from textblob import TextBlob

Second, upload the csv files that you want to analyze.
#Upload file
from google.colab import files
uploaded = files.upload()

train = pd.read_excel('tesla_sales.xlsx')
#train = pd.read_excel('2020.xlsm')
#train = pd.read_csv('train.csv')
print(train.head(10))

#For the rest of code, it will help you to create a new dataframe that contain simplified text
#Then, it will help you to provide several feature that decide the sentiment level of content from each twitter link.
