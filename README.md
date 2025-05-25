# dota_data_science

Overview
This exciting event is designed to harness the power of machine learning (ML), a branch of artificial intelligence that enables computers to learn from data and make predictions or decisions without being explicitly programmed. ML is deeply integrated into today's world and impacts various sectors. By focusing on ML techniques for this hackathon, we aim to increase the interest and expertise in ML in D&I, so we have a larger group of engineers we may leverage on future ML efforts. In addition, we can add ML to our solutions to increase their viability and effectiveness. Join us as we delve into the world of algorithms, data analysis, and predictive modeling to unlock new potentials and create impactful applications that align with Parsons' mission of delivering innovative and sustainable solutions.

The competition will be focused on predicting the winners of an eSports competition, utilizing data from the Dota2 (https://en.wikipedia.org/wiki/Dota_2) game. Data will be provided from a combination of public and private matches. Your job will be to build a machine learned model to predict whether the Radiant team will win or not.

A basic knowledge of computer programming is required for this hackathon, though you can choose from several languages to write your code in – Python, Java, or R.

The competition will run from 1100 MT on 21 Apr, and will close at 12:00 MT on 9 May. The final results will be published and a awards ceremony will be held at 12:30 MT on 9 May.

Team size maximum is five people. Feel free to mix teams of D&I employees across geographic locations and projects. You will form teams on the Kaggle platform at the start of the competition, so it would help to identify your team members prior to the competition start.

Start

Apr 21, 2025
Close
May 9, 2025
Description
In this competition your task is to predict the outcome of a selection of Dota 2 games taken from both public and professional matches, using all the game’s characteristics up to a certain point in the game. There are two teams in Dota 2 games: Radiant and Dire. You’ll need to evaluate if the team Radiant will be victorious. The game’s data is presented with various features, event logs, time series, etc. Working with game’s data and learning to see patterns and regularities can improve the ability to predict a winner.

In a regular Dota 2 game each of two teams - Radiant and Dire - consists of 5 players. For each game player chooses a hero and consequently a role. Dota 2 is a team game so the team’s composition matters. The map contains bases of each team (fountain) and 3 lanes on each side, shops, Roshan's lair and other elements.



Evaluation
Submissions are evaluated on the overall accuracy of the model using an F1-Score, (https://en.wikipedia.org/wiki/F-score) an accuracy calculation.

Submission File
For each row in the test set provided, you must predict a probability for the radiant_win variable. You will create a CSV file which should contain a header row and have the following format:

 match_id_hash,radiant_win
 abcdef1234567890abcdef1234567890abcdef12,True
 cdef1234567890abcdef1234567890abcdef1234,False
 ef1234567890abcdef1234567890abcdef123456,True
 1234567890abcdef1234567890abcdef12345678,True
 34567890abcdef1234567890abcdef1234567890,False
etc.
Since the test set contains 10000 records, your submission will also need 10000 rows. As explained in the ML overview during the kickoff, a random set of the test data is marked public, and your submission will be scored on that for the public leaderboard. After the conclusion of the competition, your submission will be re-evaluated on the private data that was held back. The final leaderboard will be published at 1230 MT on 9 May.
You may submit up to 5 files per day for testing. You may only mark one of those files for evaluation at the close of the competition.

Scoring
The F1-Score balances precision and recall. It is suitable for binary classification, especially with imbalanced datasets.
The formula for the F1-Score is:
F1-Score = 2 * (Precision * Recall) / (Precision + Recall)
Where:
Precision is the ratio of correctly predicted positive observations to the total predicted positives. The formula for precision is:
Precision = TP / (TP + FP)
Recall is the ratio of correctly predicted positive observations to all observations in the actual class. The formula for recall is:
Recall = TP / (TP + FN)
Details on the confusion matrix (TN, FN, FP, TP) can be found in the kickoff slides.

Competition Winner
The competition winner will be determined based on the highest F1-Score achieved on the private test set. The private test set consists of 5,000 matches that are not visible to participants during the competition. This ensures that the final evaluation is unbiased and prevents overfitting to the public test set.

Participants should aim to develop models that generalize well to unseen data, as the private test set scores will be the ultimate criterion for ranking and determining the winner of the competition. Therefore, it is crucial to avoid overfitting to the training or public test sets and to focus on building robust models that perform well across different datasets