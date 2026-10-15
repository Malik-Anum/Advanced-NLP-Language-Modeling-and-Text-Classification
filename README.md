# Advanced NLP: Language Modeling and Text Classification

## Project Overview
This academic project explores advanced statistical Natural Language Processing techniques, including probabilistic language modeling, smoothing algorithms, out-of-vocabulary handling, and text classification.

## Key Implementations
- Good-Turing and Simple Good-Turing smoothing
- Interpolated Kneser-Ney smoothing
- Laplace smoothing and perplexity comparison
- Out-of-Vocabulary (OOV) handling
- Multinomial Naive Bayes classification from scratch
- Learning curves and hyperparameter ablation studies
- Model evaluation and error analysis

## Technologies
Python, Jupyter Notebook, NLTK, NumPy, scikit-learn, Matplotlib.

## Datasets
- Brown Corpus
- WebText Corpus
- Gutenberg Corpus
- 20 Newsgroups Dataset

## Evaluation
The project investigates language-model perplexity, classification accuracy, precision, recall, macro-F1, and the effects of model configuration.

## Future Research
Extending statistical NLP experiments to low-resource languages and comparing traditional probabilistic approaches with modern transformer-based models.

## Project Type
Academic NLP coursework and technical portfolio project.

## Results

### 1. Language Model Perplexity Comparison

| Model | Brown Reviews | WebText |
|---|---:|---:|
| Unsmoothed Bigram | 971619.56 | 23769344.55 |
| Laplace Bigram | 3990.36 | 7179.48 |
| Laplace Unigram | 1415.08 | 3213.95 |
| Good-Turing Bigram | 6068065.81 | 39860621.91 |
| Kneser-Ney Bigram | 2530.92 | 15982.80 |

### 2. Multinomial Naive Bayes Classification

- Dataset: 20 Newsgroups (4 classes)
- Reported classification accuracy: **88.72%**
- Majority-class baseline accuracy: **25.60%**
- Random-weighted baseline accuracy: **25.60%** (single reported run)

### 3. OOV Handling Results

| Strategy | Perplexity |
|---|---:|
| Frequency threshold >= 2 | 1198.85 |
| Frequency threshold >= 5 | 462.32 |
| Open vocabulary | 4869.46 |

### Preliminary Findings

The saved notebook reports lower perplexity for the Laplace unigram model on both evaluation corpora. The four-class Naive Bayes implementation reports 88.72% accuracy, substantially above the recorded baselines. OOV vocabulary thresholds also produce different perplexity values.

**Validation note:** These figures are reproduced from saved notebook outputs and are not independently validated. Probability normalization, unseen-token handling, evaluation consistency, and model comparisons should be verified before making definitive research claims.
