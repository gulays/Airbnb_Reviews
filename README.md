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





- Tools: Pandas, Numpy, langdetect, NLTK, Matplotlib, Seaborn, sklearn, pyLDAvis

