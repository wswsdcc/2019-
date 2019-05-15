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

e.g.: 

    1,Jo bhi ap se tou behtar hoon,Negative

- Test data

 NO | column name | type | description
 -|-|-|-
 1 | ID | int | Unique ID of the text
 2 | review | string | Content of the text

## Data preprocessing

From the dataset we can learn that:
1. The language of texts is not English (According to google translation, it is Indonesian, but there are some English words mixed in it).
2. Some texts contain `\n`, e.g.:

    1095,"Wohooo just love it
    P.s: That phupii ka walima cracked me up"

3. Some texts contain emojis, e.g.:

    758,hum tu hanstay b ni 😂😂😂😂😂
    891,jab bh bolna kachra hi ugalna :)

4. The use of punctuation in text is not standardized (in order to express the tone), e.g.:

    599,Its just to provoke for jihad ..it was the biggest drama ......but flopped ...

5. There are misspellings in the text (some of them are meant to express a strong tone), e.g.:

    1594,Soooooo heartbreaking. Ya Allah in yahodyun ko gharq krdey,Negative

