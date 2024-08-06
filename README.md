### Problem Definition
What are the factors that influence customer satisfaction with the company's medicines? This is an 
issue worth addressing by the company as customer satisfaction is a key indicator of the 
effectiveness and value of the company's products. In addition, improved customer satisfaction can 
lead to increased customer loyalty and repeat business, which can have a positive impact on a 
company's bottom line.

### Type of Data Mining
This will be a text-mining task to identify patterns, words, and correlations that may indicate 
which factors are most important to customers and which areas the company could focus on to
improve satisfaction. Data collected provides us with quantitative and qualitative 
data from customer feedback.

### Dataset Source
The data set is provided from the UCI Machine Learning Repository: Drug Review Dataset (Druglib.com) 
Data Set. The dataset was compiled from online reviews from patients. It provides reviews from 
patients using specific drugs and their respective conditions. The dataset has categorical, text, and 
numeric data. It consists of multiple columns with information on the name of the drug as urlDrugName, 
the name of the condition as condition, a five-step side effect rating as sideEffects, and a five-step
effectiveness rating as effectiveness, these are all the categorical data. The 10-star patient rating 
recorded as rating is a numerical data. Finally, the text data include the patients' side effects as 
sideEffectsReview and patient benefits from the drugs they are on as benefitsReview.

### Data Preparation
Both the training and testing datasets came in '.TSV' files which stand for tab-separated values,
it is a file commonly used by spreadsheet applications to exchange data between databases as
stated by the website fileinfo.com. I converted it to a '.CSV' file with Python and exported it so I could have the CSV file saved.
After converting the file to '.CSV' I noticed a column was added that was not present in the dataset 
description. I also did not see the need for this new column called “Unnamed: 0” so I dropped it 
before proceeding. I went ahead to do some data cleaning such as checking for NAs, I only identified 
NAs in the training data set and removed them as I saw no point in generating values for people. I 
felt that would not be a true representation, and since it was a little part of the data set, I did not mind 
removing it.

Another thing I did for data preparation was on removing stopwords for wordcloud. This ensured I 
had a display of high-occurring words devoid of unnecessary words. I also went on to put the text in 
columns I used for the models I created from the various algorithms into lowercase and did some 
stemming as well. I think the stemming helped optimize the training of the models as it reduced the 
different forms of the same words that were present.

### EDA 

![Sntmt Anls 1](https://github.com/user-attachments/assets/fe5bbc10-7703-462e-8fd0-fd4d43bc0545)


