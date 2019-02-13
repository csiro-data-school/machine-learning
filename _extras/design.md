---
layout: page
title: "Lesson Design"
permalink: /design/
---
## Contributors

[Names]

We are actively seeking contributors to help with design of exercises, feeback on lessons, proofreading etc. Please submit a pull request to make your contribution.

## Process

We are loosely following the reverse instructional design process described in the software carpentry lesson template here: [reverse design] (http://carpentries.github.io/lesson-example/01-design/index.html) 

## Assumptions

**Audience:**
**Number of students:** 12
**Number of educators:** 2 + 1 helper
**Contact time:**
**Practical time:**
**Skill level:** Beginner through to lower intermediate. 
**Background:** CSIRO employees, including research scientists, technicians, and support staff. 
**Prior learning:**

## 1. Final task (Practical exercise)

### Task 
What should learners be able to do, at the end of this unit? Please describe this in one to two sentences, in terms of a practical, real-world task. 

Your task(s) should be achievable in the practical time allotted. Individual tasks should take 1/2 to 2 days. 

**Task:** Process a dataset with "issues"

**Task:** Identify existence of issues

**Task:** Fix/overcome those issues

### Data

What kind of data do learners need to bring to the workshop, to complete this task? What features should the data have? (shape, size, complexity, licence etc).

Can you design this exercise on a predesigned data set if necessary? If so, what should this dataset look like, and where can we find it from? Do we need different data for different learners?

_Ideally the data will contain a range of "issues" that can be used to illuminate particular ML concepts. Dataset issues might include:_

- _imbalanced_
- _biased_
- _noisy_
- _incomplete_
- _wide and shallow_
- _data formatting_
- _multiple files_
- _redundant features_
- _feature extraction?_

## 2. Concept map

What are all the ideas, connections, and assumptions a learner must master to achieve the task(s) described above? Please take photos of your concept maps and upload to the figures directory, with a link below.

![High level concept map](IMG_2719.jpg "High level concept map")
![Data concept map](IMG_2715.jpg "Data concept map")
![Pipelining concept map](IMG_2716.jpg "Pipelining concept map")
![Model concept map](IMG_2717.jpg "Model concept map")
![Assumptions concept map](IMG_2718.jpg "Assumptions concept map")

## 3. Episodes

Break your concept map up into smaller 'chunks'. Each new map should only contain 5-6 ideas. These form the individual teaching 'episodes' from which our larger topic unit is composed. 

Give each 'chunk' a title and link to the smaller concept map figure below. Estimate the teaching time. 

## 4. Ordering

We all know how interconnected every concept is, however teaching happens in linear time (let's debate this over dinner!). So, we now need to turn our concept networks into ordered lists. 

Start by ordering your 'chunks' or episodes. Then write each idea or concept within a chunk onto a sticky note, and order the sticky notes. Make a poster of your stick note episodes! Do you episodes fit into your teaching time? Bring it to lunch for feedback.

Once you are happy with your design, please transcribe it below. 

## 5. Exercises (formative assessments)

Each sticky note needs an exercise! Start putting your episodes into GitHub, and formulating an exercise to test / teach each concept. Keep in mind the 'data' you described back in step one. Try and keep the exercises relevant and engaging.

Keep a note of exercises / tasks that still need work here. Raise them as git issues for completion post workshop. 

## NOTES & FEEDBACK

### 1 - What is ML?
**Ep 1: Motivating Example, Counter Example**
- ML can be useful
- But you need to be careful

**Exercises:** 
- Walk through/reproduce interesting/successful ML publication/application.
- Juxtapose with an example with bad data or bad practices to illustrate what might go wrong.

**Ep 2: ML Vs. Programming**
- Traditional models are explicitly programmed.
- ML algorithms are learned.
- Therefore data is very important

**Exercises:**
- Give some examples of explicit programming
- Give some examples of machine learning

**Ep 3: Types of ML**
_No code_
- Supervised
- Unsupervised
- Classification
- Regression
- Deep learning

**Ep 4: Why to ML?**
- Data vs. knowledge
- Predicition vs. understanding
- Interpretability
- Applications in science and industry (with examples)

**Ep 5: When to ML?**
- Data requirements
- Compute requirements
- Desired outcomes

**Ep 6: How to ML**
- Frameworks
- Tools (hardware and software). Data processing, data pipelining.

### 2 - Data Pipelines and ETL (Extraction, Transformation and Loading)
**Ep 1: Data**
- Data collection
- Data types (labelled vs unlabelled, time series)
- Data formats
- Big Data
- _(with examples)_

**Ep 2: Getting and Viewing Data**
- Loading
- Downloading
- Streaming
- Loading big data?
- Data visualisation/inspection

**Exercises:**
- Visualise data

**Ep 3: Data Munging**
- Reshaping
- Joining

**Exercises:**
- Visualise changes
- Apply ML model

**Ep 4: Tidying Data**
- Cleaning
- Normalisation / Standardisation
- Outliers
- Noise

**Exercises:**
- Visualise changes
- Apply ML model

**Ep 5: Feature Engineering**
- Types of features
- Dimensionality
- Feature engineering
- Choosing features / which features to use

**Exercises:**
- Visualise changes
- Apply ML model

**Ep 6: Data Augmentation**
- Augmentation
- Resampling
- Oversampling

**Exercises:**
- Visualise changes
- Apply ML model

**Ep 7: Data Pipeline (optional?)**
- Automated pipelines
- Checkpointing

**Ep 8: Recipe**
_not necessarily code_
- Data pipeline template / workflow
- Not necessarily linear
- Most likely iterative

**Exercises:**
- Pipeline Ep 1 - 6

### 3 - ML Models
**Ep 1: Types of ML Algorithms**
_with code_
- Supervised
- Unsupervised
- Parametric vs. Non-parametric
- Instance based (lazy)
_with code examples_

**Ep 2: Types of ML Problems**
_with code_
- Classification
- Regression
_with code examples_

**Ep 3: Looking inside the Black Box**
- Explain simple model (kNN) in detail
- Use to illustrate complexity of ML
- Introduce concept of hyperparameters

**Exercises:**
- Determine hyperparameters for the kNN implementation in scikit-learn
- Potentially summarise some classic literature?

**Ep 4: Training / Learning**
- Louie/Not Louie thought experiment
- Batch
- Epochs
- Gradient descent (or something)

**Ep 5: Recipe**
- Builds on Pipeline recipe

### 4 - Testing and Verification
**Ep 1: Introduction**
- Motivating examples illustrating importance of testing

**Ep 2: Metrics for Performance**
- Different metrics (precision, recall, F-score, etc)
- Metric visualisation (confusion matrix, ROC curves)
- What problems can these metrics identify?

**Ep 3: Overfitting**
- How to identify overfitting
- How to fix overfitting
- Introduce model complexity and it's relation to overfitting

**Ep 4: Validation and Hyperparameter Tuning**
- Train/val/test splitting
- Cross validation
- Hyperparameter tuning
- Hyperparameter sensitivity (overfitting)

**Ep 5: Recipe**
- Full pipeline
- Includes loading, training and validating.
