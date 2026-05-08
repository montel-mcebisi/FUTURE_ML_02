# FUTURE_ML_02
Future Interns

I started off by uploading my csv file into a pandas dataframe, and displayed my data.
Took on to understanding my datset, getting the shape, the necessary info and described my data and found that it had 2 columns and luckily there were non-null entries in all my rows and columns.
Found the count for all my data, the most unique categories and the top category "Hardware" and its frequency and found it made up 28% of my data.

I used tools such as matplotlib and seaborn to count and plot so that i can see how my ticket volume was distributed, a count plot was generated that showed how my categories were distributed.

I imported Natural Language ToolKit, and filtered words such as "is","the", "a" (stopwords) out of my data. I also removed punctuation whilst at it.

I went on to turn my text into numbers using Vectorization from tool sklearn .
I got my TF-IDF (How often a word appears in a specific ticket)
Turned the Document column into a mathematical matrix that our model would later use.
TfidfVectorizer mutes unnecessary non-technical words and boosts score fore techincal one.

Used LabelEncoder to turn target categories into numbers

Divided my data and used "train_test_split", where 20% I had a 20% test split and trained 80%.

Used a Multinomial Naive Bayes model for baseline text classifications as it works specifically by calculating word probabilities across diff categories, This looks at the words in a ticket and calculates the probability of that ticket belonging to "Technical" or "Hardware"

Finally, Set a Business Logic for Priortiy with "Hardware as our top priority followed by "Access", "Purchase", etc.




