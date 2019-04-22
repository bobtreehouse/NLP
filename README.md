# NLP
sample project using Natural Language Processing, NLTK, word scrapers, stop-words, some pandas merge and concat and matplotlib.
**Trouble with my code** 
 - I had some difficulty after cleaning the text, converting the results of the "word count" which were in ``` list ``` form and 
 converting that to its own ```dataFrame ```.
   - this was the key line to fixing that **===>** ``` df3=pd.merge(df1, df2, on ='words', left_index=True) ```
 - I struggled to get the actual "Term Labels" from column 0 of the dataFrame onto to the horizontal bars in the vizualization step.
 - I played around with adding a WordCloud but do not think I emplemented it correctly. 
 
 I performed a text scrape of the full minutes from both the Dec 2018 FOMC statement with the subsequent Mar 2019 FOMC statement, 
 cleaned the text and then performed a word count to look for key differences in trigger words that market participants look for to 
 signal the Feds intentions of forward rate paths.
 
**Observations** In the March 2019 statement, We could observe a higher count of words ``` Risks ``` , ``` Uncertainty ``` and 
``` Projections ``` . Additionally, the March 2019 saw the introduction of the word ``` Subdued ``` , which was completely absent 
from the previous December 2018 statement.
