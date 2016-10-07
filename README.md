# indeed
Katya's Project 4
In this project I analysed Data Science jobs advertised on www.indeed.com. I scraped around 40K data science ads from the site and split them into bins by salary:
'junior' - salary range 55-70K
'middle-low' - salary range 70-85K
'middle-high' - salary range 85-100K
'senior' - salary range 100-115K
Then by means of Natural Language Processing Python library I did analysed (tokenized) all the words and found those ones which could be used as a markers for the corresponding salary bins.
Then I built Logistic Regression model which allows determining probable salary range. This might be helpful for job seekers to assess any particular Data Science job description and forecast the salary offered by company or match their expectations with the current Data Science Labour market tendency.
Outline:
scraping data: I scraped 39959 positions from www.indeed.com in equal proportion for each bin. So we can assume that the data set is balanced.
binning: by salary
cleaning data: I removed all the stopwords(commas, zero-meaning words, etc.)
parsing data: tokenizing, finding bigrams, most_common words for each bin
building model
evaluating model