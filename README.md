# Automatic Grading System
An AI based automatic grading system implementation in TF 2.0.

## Inspiration

The online exams are kicking for coding exams and MCQ type questions where output and answers are foreknown respectively. There is no facility for online exams for schools, colleges etc. where the answers are subjective to the question due to the reason that there is no particular answer for such questions. Lot of hardwork and time is also required by the teachers to check such answers.

## What it does

The system allows online exams for subjective questions by automating the process of grading (checking) subjective (comprehensive) answers with the help of AI. Thereby motivating school/college institutes to conduct exam online. The students can give the exam through web portal at home or computer labs at institute. 

## How we built it 
The project has 3 phases:
feature extraction,Label scaling and training with Neural network.
#### 1. Feature extraction
We extracted 11 features which are used for statistical and theoretical aspects of the answer. 
##### a. Statistical features:
Word count, Vocabulary count, Noun count, Verb count, Adverb count, Adjective count. Sentence length and Wrong spelling% 
##### b. Logical features 
Bag of words, perplexity feature (tells extent to which essay is related to topic asked in question) and beautiful words count. 

#### 2. Scaling of target variable 
Target variable is scaled separately for each comprehension set as each comprehension has different maximum and minimum grades.

#### 3. Neural network
The system uses Tensorflow 2.0 to train the dataset available by Hewlett Foundation. The model has 2 hidden layers and 200 neurons in each layer.

## Challenges we ran into
* Feature extraction and removing biases. 
* Standardising labels. 
* Changing the target variable.

## Accomplishments that we're proud of
* The final loss came out to be 0.1856. 
* The testing was also conducted on various subjective questions with good results.

## What we learned
A good grasp on NLP and feature extraction 

## What's next for Automated Grading System
To scale the project to grade the non subjective answers like using numerical formulas and technical stuffs.
