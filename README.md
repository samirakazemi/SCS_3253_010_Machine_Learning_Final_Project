# SCS_3253_010_Machine_Learning_Final_Project
Repository dedicated to Final Project of UofT Machine Learning Course.



[![Google Colab](https://avatars2.githubusercontent.com/u/38081706?s=60&v=4)](https://colab.research.google.com/github/samirakazemi/SCS_3253_010_Machine_Learning_Final_Project/blob/master/Final_Project.ipynb)


Team members:


| Name | Github Repo |
| --- | --- |
| Engy Abdel Azeez  | https://github.com/engy369 |
| Armin Jamshidi | https://github.com/arminjamshidi |
| Samira Kazemi  | https://github.com/samirakazemi |
| Shahzeb Shahid | https://github.com/sshahid09 |


The purpose of this analysis is to look into the Poker Hand Data set and analyze the strength of each hand as a classification exercise. This dataset has already been divided into two sets of train and test sets. Hence there is no need to split the data before starting the analysis.

**Dataset description:**

Each record of the dataset consists of five playing cards. In poker game, each hand consists of 5 cards drawn from a standard deck of 52. Each card has two attributes:
- rank
- suit

This will give us 10 predictive attributes for each poker hand. There is one Class attribute that describes the Poker Hand.


**Attribute information of each card in one poker hand as described in UCI:**

1) S1 "Suit of card #1" Ordinal (1-4) representing {Hearts, Spades, Diamonds, Clubs}
2) C1 "Rank of card #1" Numerical (1-13) representing (Ace, 2, 3, ... , Queen, King)
3) S2 "Suit of card #2" Ordinal (1-4) representing {Hearts, Spades, Diamonds, Clubs}
4) C2 "Rank of card #2" Numerical (1-13) representing (Ace, 2, 3, ... , Queen, King)
5) S3 "Suit of card #3" Ordinal (1-4) representing {Hearts, Spades, Diamonds, Clubs}
6) C3 "Rank of card #3" Numerical (1-13) representing (Ace, 2, 3, ... , Queen, King)
7) S4 "Suit of card #4" Ordinal (1-4) representing {Hearts, Spades, Diamonds, Clubs}
8) C4 "Rank of card #4" Numerical (1-13) representing (Ace, 2, 3, ... , Queen, King)
9) S5 "Suit of card #5" Ordinal (1-4) representing {Hearts, Spades, Diamonds, Clubs}
10) C5 "Rank of card 5" Numerical (1-13) representing (Ace, 2, 3, ... , Queen, King)
11) CLASS "Poker Hand" Ordinal (0-9)

**Attribution of the strength of the hand as described in UCI:**

0) Nothing in hand; not a recognized poker hand 
1) One pair; one pair of equal ranks within five cards 
2) Two pairs; two pairs of equal ranks within five cards 
3) Three of a kind; three equal ranks within five cards 
4) Straight; five cards, sequentially ranked with no gaps 
5) Flush; five cards with the same suit 
6) Full house; pair + different rank three of a kind 
7) Four of a kind; four equal ranks within five cards 
8) Straight flush; straight + flush 
9) Royal flush; {Ace, King, Queen, Jack, Ten} + flush"

# Our approach

We first started with Data Preparation and Pre-prediction Exploratory Data Analysis. For that we made use of functions such as “_describe( )_” which helps to view some basic statiscital details of our data set, “_shape_” which returns the dimesions of our dataset, “_info_” which gives the summary of our dataset and “_head( )_” which shows the data of the top five rows from our dataset. We have also plotted the histogram for each of our test and train dataset. The results of this exploratory analysis allowed us to become familiar with our dataset before starting the pipeline process.

To build the pipeline, the data were normalized using “_StandardScaler( )_”. This function helps us to make sure that all of our dataset features have the same weight and importance.

Since the category membership of our dataset is known, we are going to use the classification technique on our dataset. We have used models such _KNN_, _SVM_, _RandomForest_, _Adaboost_, _Gradient Boosting_ and _Bagging_ to analyze the dataset, find their accuracy and predict the labels.

Before fitting the data into the models, hyperparameters were used to train the data even more effectively.

The accuracy of each model was plotted and the results show that _ has the highest acuuracy to predicate the correct strength of the poker hand compared to other models that we have used.

**Here is a quick walkthrough of our project:**

[![Video](https://img.youtube.com/vi/YQPSk7zC2bU/0.jpg)](https://www.youtube.com/watch?v=YQPSk7zC2bU)
