# Spark_NLP
Our project started with installing PySpark and opening the session. We then read the data, which consisted of testimonials pulled from IMDb, and moved on to the exploration phase.

In this step, we understand the organization of our database by checking the number of rows and columns, in addition to their content. Next, we learned how to filter comments and ended up counting testimonials with positive and negative feelings.

Familiar with our set, we move on to the data cleaning step. We made a word cloud in order to check the most frequent words and we removed some special characters using regular expressions (Regex). Then, we split the comments into small parts using the concept of tokenization. Finally, we remove the stop words, or empty words.

After cleaning the data, we applied vectorization, which is the creation of a bag of words, from CountVectorizer, which allowed us to observe the peculiar structure of the bag of words. We are also aware of HashingTF as an alternative for creating this bag of words, a method that even allows us to limit the vocabulary. To finalize this vectorization, we use TFDF to apply weights to the words in order to identify the most relevant ones.

Then, we apply one more transformation, this time to the response variable, coding the original categorization of the comments. That done, we condensed all this transformation into a Pipeline function, which optimizes the process and facilitates execution.

After processing, transforming and vectorizing our data, we started our first model by identifying the problem and the methodology that would best correspond to the desired solution, the decision tree. We then filter our data and fine-tune our pipeline including the decision tree as one of the steps to take. We also defined our training and test bases, which allowed us to understand how our model performed by applying the accuracy metric.

To finalize the project, we include a dataframe of two comments, one negative and one positive, in order to verify how our model would classify them. The classification matched the categorization of the testimonials, so our model worked!
