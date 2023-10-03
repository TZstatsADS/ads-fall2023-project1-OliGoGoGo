# Applied Data Science @ Columbia
## Fall 2023
## Project 1: What made you happy today?

![image](figs/title.jpeg)

### [Project Description](doc/Proj1_desc.md)
This is the first and only *individual* (as opposed to *team*) this semester. 

Term: Fall 2023

+ Projec title: Marriage impacts happiness level among different people?
+ This project is conducted by Olivia

+ Project summary: We have already gotten the source where people's happiness come, but I'm curious about the activities which can drive people happier, and try to get some conclusions on it. In general, the goal of this project is to analyze the distribution of these happiness levels to understand how people express their happiness in various degrees.

+ HappyDBFindings
In this project I will carry out an exploratory data analysis of the corpus of [HappyDB]([url](https://megagon.ai/happydb-a-happiness-database-of-100000-happy-moments/)) and write a blog on interesting findings.

Texts are explored using tools from text mining and natural language processing such as sentiment analysis, topic modeling, etc, all available in R and write a blog post using R Notebook. 
 
The blog will be in the form of a data story blog on interesting trends and patterns identified by the analysis of these happy moments.


+ Project Steps:

1: Data Collection & Preprocessing:

   Clean the dataset by removing irrelevant and noisy data.
   Perform text preprocessing tasks: tokenization, stop-word removal, and lemmatization.

2: Exploratory Data Analysis (EDA):

 2.1: Generate summary statistics: the distribution of happiness levels, and common keywords or phrases.

 2.2: Word Clouds and Keywords:

      Generate word clouds to highlight the most frequently mentioned words or phrases associated with happiness.
      Identify interesting keywords and phrases that appear in the happy moments.

3: Sentiment Analysis:

   Apply sentiment analysis to classify the happiness levels of the moments 
   Visualize the distribution of happiness levels in the dataset.

4: Topic Modeling:(word2Vec)

   Visualize the topics and prevalence in the dataset


5: StoryLine and Insights & Findings:

   5.1: the distribution of the length of texts' key contend is relatively concentrated and skews to the right:
        5.1.1: Concentrated may suggest: 
           people's levels of happiness are relatively consistent.
           The observed values are subject to certain constraints or conditions, leading to limited variations within a specific range
        5.1.2: Skews to the right may suggest:
           A common phenomenon in emotion research is that people tend to share and document positive experiences more frequently, while sharing negative emotions less often. 
           HappyDB may contain a higher proportion of topics related to positive emotions and happiness.
           The sampling method of the dataset may have resulted in the selection of more positive samples, introducing sampling bias.
   
   5.2: the combination of marital status and gender has significant influence on happiness
        5.2.1: Sequence of events:
           the happiness distribution by marital status shows a little difference between different group;
           further, I added one more feature into it and performed ANOVA analysis to see the impact
           Assumption0: marital status and gender don't have significant impact on happiness level
           I got an extremely small p value, which contribute to refusing the 0 assumption;
           To get more details about it, I did a heatmap, to show the difference
        5.2.2: separated male shows the highest level of happiness while widowed male shows the lowest level of happiness
           This finding is interesting, and I think we can dig more about it


   5.3: use v2w, got drinks related, among all the drinks, coffee got the most popularity

6: Conclusion and Reflection:

   6.1: Key findings and insights shown in 5
   6.2: Through this project, I reflect on the significance of understanding and celebrating moments of happiness.
   6.3: This project not only provide valuable insights into the HappyDB dataset but also allow me to practice data mining, statistical analysis, and data storytelling skills.
   6.4: There are still many areas worth improving and exploring further, for example, the sentiment analysis results are not specificated enough, we may use more sophiscated methods to upgrade the model; word2vector model are not gotten leverage it's real charm, may use it to do more work; the ANOVA results can get further researched, to see if different features are working on each other; the drinks part is a bit funny, just as an addition 




Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
