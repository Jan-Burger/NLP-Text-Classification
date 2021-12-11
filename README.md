# NLP-Text-Classification

## Abstract
Traditional machine learning models have been around for
many years. Since computing power has grown a lot over the years, the
preferred method for machine learning nowadays are neural networks.
Since the rise of neural networks, traditional machine learning models
have moved into the background of research. That’s why in this paper
I want to focus on the traditional approach of machine learning and
ask the question of which traditional machine learning model has the
best performance on the task of text classification of twitter data. My
research is based on the data set of Thomas Davidson, Dana Warms-
ley, Michael Macy, and Ingmar Webe[4]. In the first step, I used typical
preprocessing techniques like the removal of punctuation to prepare the
data for the machine learning model. I then did some Exploratory Data
Analysis to get insight to the data and extract new features. After that I
tested different possibilities to train and test the machine learning mod-
els like using new features or testing whether the Z-normalization does
make a difference in model performance. The traditional machine learn-
ing model with the best performance was the Logistic Regression with
94,3% accuracy.

## 1 Introduction
Traditional machine learning models are algorithms which already exist for a
long time and are very well researched and documented. In contrast to that
none traditional machine learning refers to newly developed algorithms which
at the moment most research is done with. In this paper, I want to demonstrate
the differences between traditional machine learning models and determine their
performance. All of this will be done using the example of text classification of
twitter data.
My work is based on the paper of Thomas Davidson, Dana Warmsley, Michael
Macy, and Ingmar Webe[4]. I will use their dataset of roughly 24 thousand ex-
tracted and classified tweets from Twitter to train and evaluate my machine
learning models. In their original paper, they labeled the tweets in three differ-
ent classes, 0 - hate speech 1 - offensive language 2 - neither. One big problem
arises when doing research on hate speech. The definition of hate speech varies a
lot in different papers. Fore example, one definition a research paper gave was the
following: ”HATE: This class contains tweets which highlight negative attributes
or deficiencies of certain groups or individuals. This class includes hateful com-
ments towards individuals based on race, political opinion, sexual orientation,
gender, social status, health condition etc.”[6].Another paper gave the following
definition: ’Hateful: this class includes tweets which are offensive, and present
hate, racist and segregative words and expressions.”[7]. This shows that there is
not a formal definition for hate speech. Different papers give different definitions
on what hate speech is. The research paper which my work is based on itself[4]
states that hate speech is directed towards a group of people and the goal is to
harm them in some way.
Since the definition of hate speech is not clear yet, I decided to summarize the
two categories hate speech and offensive language and call them offensive lan-
guage+. This category consists of all the tweets which in the original paper[4]
were labeled as hate speech or offensive language. My second category will sim-
ply be the tweets which were labeled as normal.



