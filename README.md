## Task of the Contest
[Introduction on the official website](https://www.kesci.com/home/competition/5cb80fd312c371002b12355f)
### Task
Establish a text sentiment classification model based on the provided training set, and predict the text sentiment in the test set by judging whether the emotion is "Negative" or "Positive".
### Dataset
- Training data

 NO | column name | type | description
 -|-|-|-
 1 | ID | int | Unique ID of the text
 2 | review | string | Content of the text
 3 | label | string | Sentiment of the text

Example: 

    1,Jo bhi ap se tou behtar hoon,Negative

- Test data

 NO | column name | type | description
 -|-|-|-
 1 | ID | int | Unique ID of the text
 2 | review | string | Content of the text

## Data preprocessing
