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
* Posts of more than 5000 users.
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

# System Requirements
# Python 3.10.0
 Python can be used for many kinds of software development. It offers strong support for
 integration with other languages and tools, comes with extensive standard libraries.
 
# Jupyter Notebook v4.11
 The Jupyter Notebook is an open-source web application that can be use to create and
 share documents that contain live code, equations, visualizations, and text. Jupyter Notebook
 is maintained by the people at Project Jupyter
# Hardware Requirements
 • RAM:Atleast 12-16 GB of RAM is required.
 • Storage: The model training and implementation may require a maximum of 10 GB of
 storage.
 • Processor: A multi-core processor with at least 2 GHz clock speed is needed.
 • GPU/TPU: An optional graphical processing unit or tensor processing unit can increase
 processing speed

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
