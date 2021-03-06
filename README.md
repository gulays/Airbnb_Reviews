# Airbnb Topic Modeling for Reviews

The project will conduct topic modeling for Airbnb Guest Reviews to identify the factors affecting guests' positive and negative experiences.

Reviews are essential to each party of the vacation rental marketplace, they help guests choose their travel plans wisely while they enable hosts to open their homes with 
more confidence. 
In addition, reviews provide a social proof of the listing quality for guests. On the other hand, for hosts more positive reviews mean a higher ranking in Airbnb search and 
attracting more guests.

## Data and Approach 

The data, Reviews is collected from Inside Airbnb and cover more than 80K reviews in New York City, till September, 2021. It includes a unique id for each reviewer and detailed comments.

### Data Cleaning:

- Remove numbers,  capital letters and punctuations,

- Eliminate non-English reviews.

- Update the stop word list by removing common words. 

- Lemmatize with TF-IDF Vectorizer/CountVectorizer

### Baseline Models : 

- NMF 

- SVD

- LDA

- CorEx


### Final Model:
Keywords for 15 topics are identified using LatentDirichletAllocation with Count Vectorizer via pyLDAvis, then each topic is labelled as follows:
Topics
- Rental interior 
- Kitchen 

- Overall Airbnb Experience

- Neighborhood- accessibility to transportation

- Home-like comfort/experience

- Neighborhood/ accessibility to dining, social attractions

- Cleanliness

- Host-hospitality

- Location- safe/family friendly

- Bed/Bathroom

- Overall trip experience

- Host-responsiveness

- Convenience (check in/out, comfort, hotel like)

- Comfort/Value

- Listing Accuracy


### Topics with the highest marginal distribution 

House Related Topics:

- Rental interior

- Kitchen

- Overall experience

- Bed/Bathroom

Location Related Topics :

- Transportation 

- Dining, social attractions

- Kid friendly, safe

Host and Listing Related Topics:

- Hospitality  

- Responsiveness

- Listing 


###  Reviews : Sentiment Analysis/ VaderSentiment 

VaderSentiment Analysis is applied to detect negative and positive reviews. It is found that most guest had pleasant experiences during their Airbnb stays as review sentiment scores are highly positives. Most common words in negative and positive reviews are revealed that host attitude, being close to subway and cleanliness are the top topics talked in reviews. 




## Tools

Pandas, Numpy, langdetect, NLTK, Matplotlib, Seaborn, sklearn, pyLDAvis

## Communication

AirbnbReviews_presentation.pdf is the presentation of the project. Airbnb.ipynb is the final Jupyter notebook.
