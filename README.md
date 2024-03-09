__Recommender system for craft beers using data scraping, natural language processing (NLP), sentiment analysis, and machine learning techniques.__ __The system uses user-generated reviews from BeerAdvocate to understand user preferences for different beer attributes and offer personalized recommendations.__

__INPUT__:
  <br>As a user you can input beer attribute you like in a beer for example dark, hoppy, malty, roasted, sweet, coffee etc.<br>
__SIMILARITY ANALYSIS__: <span style="color🟪 ;"> How similar are my attribute with the reviews? </span>
  <br>  Recommender system will do a cosine similarity analysis with the reviews using 'bag of words' approach (ti-idf vectorize) & 'word to vector' (Spacy) to recommend beers with highest similarity score.<br>
__SENTIMENT ANALYSIS__:  <span style="color🟪 ;"> Do the reviews have positive sentiment or negative? </span> 
  <br>We wouldn't want to recommend beers with negative sentiment. We calculate the sentiments score for each review unsing VADER and calculate an evaluation score using similarity & sentiment score.<br>
__ASSOCIATION ANALYSIS__:<span style="color🟪 ;"> Are beers with positive association to a common attribute similar? </span>
  <br>  We calcluate the lift of top 4 beer attributes like sweet, dark, chocolate,light with 10 beers and identify which beers have similar attribute.<br>
__OUTPUT__: 
<br>Recommend Top beers based on user reviews<br>



Following libraries were used:

- BeautifulSoup: For web scraping.
- pandas: For data manipulation and analysis.
- NumPy: For numerical operations.
- Spacy: Text embeddings
- NLTK (Natural Language Toolkit): For text processing
- Vader : sentiment analysis.
- Scikit-learn: For feature extraction and similarity computation.
- mlxtend : Apriori association
