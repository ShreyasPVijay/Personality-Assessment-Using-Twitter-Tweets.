# Introduction
This is a *machine learning* project. This trained machine learning classifier can predict a person's **MBTI**(Myers–Briggs Type Indicator)
personality type using an individual's *social media posts* like **twitter posts**.  By leveraging machine learning models to classify Twitter users
 based on their MBTI personality types, this project explores the potential for enhancing user experience and engagement on the platform, opening avenues for personalized content delivery and community building in the digital space
 
### About MBTI
The Myers Briggs Type Indicator (or MBTI for short) is a personality type system that divides everyone into 16 distinct personality types across 4 axis:
* **Introversion** (I)/**Extroversion** (I)
* **Intuition** (N)/**Sensing** (S)
* **Thinking** (T)/**Feeling** (F)
* **Judging** (J)/**Percieving** (P)
<br>
You can read more about the MBTI test [here](https://en.wikipedia.org/wiki/Myers-Briggs_Type_Indicator).

### Dataset
The dataset on which this classifier is trained, contains around 50 posts per user about 8000 users with their *MBTI*
personality type known. Dataset is provided in the repo itself personality-test.csv.
<br>
Few features of dataset are:
* Posts of more than 8000 users.
* Last 50 posts per user, each entry is separated by '|||'.

### Caveats
We have trained individiual classifier for each characterstics pair. Although script's final prediction will be complete MBTI type, the first 2
pairs/models i.e. Introversion/Extroversion and Intuition/Sensing are not reliable at any level, due to the fact that data regarding these characterstics
is heavily biased towards single attribute. For more explanation or better understanding, look at this jupter notebook.


# Usage
```
python3 main.py <username>
```
**NOTE**: **&lt;username&gt;** is twitter handle of target user(without @)

# Dependencies
* python 3.x
* numpy
* pandas
* matplotlib
* sklearn
* nltk
* colorama

# Conclusions
 Our Twitter personality detection system successfully harnessed the power of diverse
 machine learning models, demonstrating efficient accuracy across various personality dichotomies.
 The strategic reduction of MBTI classes from 16 to 4 enhanced model efficiency. The
 preprocessing phase played a crucial role in refining the raw textual data, ensuring that the
 models focused on meaningful content. By utilizing various models, we explored a multimodal-binary class approach, allowing
 each model to specialize in discerning distinct personality traits. The Confusion Matrices
 further illuminated the models’ strengths in capturing nuanced patterns within the Twitter
 account posts
