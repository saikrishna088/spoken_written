# spoken_written
converting English sentence from spoken to written
### Note:
I have not done creating Library as I am ran out of time(to learn) as I am not familiar with dealing github .But I have completed the task and uploded as .ipynb file. Sorry for the truble.please have a glance at my solution.

### Here is Explanation of the solution:
1. My approach is to classify the words into categories(Numericals,plain,Digital,Letters).
* Numericals: Includes all types of texts having numberical form like address,telephone.
* Plain: same text as output.
* Digital:web addresses and other symbols
* Letters for abbrivation like n a s a :NASA
2. First I have build a Bi-directional LSTM for the label prediction (Pedicting label for eachtoken(word)).
3. next I build seperate LSTM models for each class and got accuracy (99% for Number class,98% for Letter class,85% for Digit class).

## Feature Engineering
1. I have tried brute force LSTM for all,But got less accuracy
2. I have tried classical ML model randomForest and XGboost for classification of tokens (got 94% accuracy).
3. I have tried word level embedings which ave me good results

4. I Feel charecter level word embedingd will improve the performence of the model
5. Having more classes will also improve the model.

## Sample text result:
* input:"many people told me that having son is better than having daughter . when i was five years old playing with three of my friends we found fifty five hundred dollar note and thoughts to share among us . but unfortunatel it was taken by sixty year old men who lives in u.s and he works in n a s a."

* Predicted: "many people told me that having son is better than having daughter . when I was 5 years old playing with 3 of my friends we found 56 dollar note and thoughts to share among us . but unfortunatel it was taken by 60 year old men who lives in U.S and he works in NASA."



