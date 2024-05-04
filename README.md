# Team_6_NLP
Classifying Social Media Texts into MULTIPLE Hate-BASED Categories for Indian languages

## Problem Statement 
Developing an effective system for hate speech detection and categorization in Hindi by leveraging Hindi WordNet for initial positive and negative word scores, and subsequently expanding the lexicon using Sysnet. This approach addresses the challenge of limited sentiment analysis tools tailored for Hindi, ensuring a more comprehensive understanding of linguistic nuances and cultural contexts.

### Proposed Pipline 
- Subjectivity Analysis: The process of subjectivity analysis involves identifying subjective tweets and filtering out objective content, laying the foundation for hate speech detection.
- Building a Hate Speech Lexicon: The algorithm involves constructing a lexicon of negative words and hate verbs to accurately identify hate speech, enhancing the precision of detection.
- Identifying Theme-Based Nouns: The inclusion of theme-based nouns ensures that hate speech is contextually relevant, capturing politically significant words and other relevant nouns.

#### Subjective Analysis
- Subjectivity analysis simplifies the corpus by focusing on subjective tweets, which are more likely to contain hate speech, rather than objective ones.
- We utilize Hindi WordNet to assign positivity and negativity scores to words in the dataset.
- Using the SUBJCLUE lexicon, we match each key to its appearance in the dataset and assign corresponding positive and negative scores.
- The total score for each tweet or sentence is determined based on these assigned scores.
- Objective tweets are identified and marked as "not hate" by filtering out those with low subjectivity scores.
- We used a variety of values as the limiting values that make a tweet worth investigating further, and decided that all tweets with a score above 1.0 or below -0.5 were subjective enough to be heavy contributors towards hate speech.
- The lower limit is numerically lesser than the upper one because we found that the sentences marked negatively by the word sentiment analysis were more likely to contain hate speech.

![image](https://github.com/chaitanyabalajireddy/Team_6_NLP/assets/91625648/6e3f9247-34fb-4800-88eb-097deac67f42)




