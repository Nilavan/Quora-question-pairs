<h1 align="center">Quora question pair similarity</h1>

## About Quora and the question pair problem

Quora is a place to gain and share knowledge—about anything. It’s a platform to ask questions and connect with people who contribute unique insights and quality answers. This empowers people to learn from each other and to better understand the world.
Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

> Credits: Kaggle

## The task

- Predict whether a pair of questions are duplicates or not.
- This could be useful to instantly provide answers to questions that have already been answered.
- This is a binary classification problem

## Business objectives and constraints

- Cost of mis-classification can be high
- Interpretability is partially important
- No strict latency concerns

## Data overview

- Data is in [Train.csv](train.csv)
- 5 columns:
  - qid1 - ID of question 1
  - qid2 - ID of question 2
  - question1
  - question2
  - is_duplicate - Target 0 if questions are not similar and 1 if they are
- Number of rows - 404,290

## Performance metrics

- log-loss
- Binary confusion matrix
