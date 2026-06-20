# Skill Graph Clustering & Learner Segmentation using Unsupervised Learning

## Executive Summary

This project develops an AI-driven Skill Gap Analysis System for identifying student strengths, weaknesses, learning gaps, and future learning needs. The system applies K-Means Clustering for learner segmentation, Association Rule Mining for discovering related skills, and Random Forest Regression for predicting future skill proficiency. Personalized learning recommendations are generated to support student growth and improve learning outcomes.

---

# Dataset Overview

### Dataset Information

* Dataset Name: Task11_dataset.csv
* Total Records: 2000
* Total Students: 200
* Total Skills: 20
* Skill Categories: Programming, AI, Analytics, Visualization, Database, Cloud, Security, Tools, Development

### Features Used

* Student_ID
* Skill_Name
* Skill_Score
* Assessment_Score
* Course_Completion_Percentage
* Learning_Hours
* Assignment_Completion_Rate
* Login_Frequency
* Skill_Category
* Proficiency_Level

---

# Data Preprocessing

The following preprocessing steps were performed:

### Missing Value Handling

* Checked for missing values.
* No significant missing values were found.

### Duplicate Removal

* Duplicate records were identified and removed where applicable.

### Feature Encoding

Categorical columns encoded using Label Encoding:

* Skill_Name
* Skill_Category
* Proficiency_Level

### Feature Scaling

StandardScaler was applied to:

* Skill_Score
* Assessment_Score
* Learning_Hours
* Login_Frequency

---

# Exploratory Data Analysis

The following visualizations were created:

### 1. Skill Distribution Analysis

Displays overall distribution of student skill scores.

### 2. Skill Gap Heatmap

Shows skill gaps across students and skills.

### 3. Cluster Visualization

Displays learner segmentation generated using K-Means Clustering.

### 4. Correlation Matrix

Shows relationships between learning features and skill performance.

### 5. Recommendation Dashboard

Displays recommended learning paths.

### 6. Future Skill Prediction Graph

Compares actual and predicted skill scores.

---

# Skill Gap Analysis

Skill gap was calculated as:

Skill Gap = 100 - Skill Score

### Strong Skills

Skills with higher average proficiency scores represent strong competencies among students.

### Weak Skills

Skills with lower average proficiency scores indicate learning gaps and areas requiring additional focus.

### Missing Competencies

Students with large skill gaps were identified for targeted learning interventions.

---

# Learner Segmentation using K-Means Clustering

## Objective

Group students based on learning behavior and skill performance.

### Input Features

* Skill_Score
* Assessment_Score
* Learning_Hours
* Login_Frequency

### Clusters Generated

* Beginner Learners
* Intermediate Learners
* Advanced Learners

### Evaluation Metric

Silhouette Score was used to evaluate clustering quality.

The clustering model successfully segmented students into meaningful learner groups.

---

# Association Rule Mining

## Objective

Identify skills that are frequently learned together.

### Technique Used

Apriori Algorithm

### Outcomes

The model discovered:

* Frequently learned skill combinations
* Related learning paths
* Skill dependencies

These insights can help build personalized learning recommendations.

---

# Future Skill Prediction

## Objective

Predict future skill proficiency.

### Model Used

Random Forest Regressor

### Evaluation Metrics

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* R² Score

The model demonstrated the ability to estimate future student skill performance based on historical learning behavior.

---

# Personalized Learning Recommendations

Recommendations were generated using current skill proficiency levels.

### Recommendation Strategy

#### Beginner Path

Recommended for students with low skill scores.

Focus Areas:

* Basic concepts
* Practice exercises
* Foundation courses

#### Intermediate Path

Recommended for students with moderate proficiency.

Focus Areas:

* Applied projects
* Advanced exercises
* Skill reinforcement

#### Advanced Path

Recommended for highly proficient students.

Focus Areas:

* Specialization
* Industry projects
* Expert-level topics

---

# Business Questions and Answers

## Q1. Which skills demonstrate the highest proficiency among students?

Skills with the highest average skill scores were identified through aggregation and ranking.

## Q2. Which skill areas have the largest learning gaps?

Skill gap analysis identified areas with low proficiency and high improvement potential.

## Q3. Can students be grouped based on their skill profiles?

Yes. K-Means Clustering successfully grouped students into learner segments.

## Q4. Which machine learning technique best identifies similar learning patterns?

K-Means Clustering effectively identified students with similar learning behaviors.

## Q5. What personalized learning paths should be recommended?

Beginner, Intermediate, and Advanced learning paths were generated based on proficiency levels.

## Q6. Which skills are frequently learned together?

Association Rule Mining identified common skill combinations and dependencies.

## Q7. Can future skill proficiency be predicted?

Yes. Random Forest Regression successfully predicted future skill scores.

## Q8. How can personalized learning paths improve outcomes?

Personalized recommendations help students focus on learning gaps, improve proficiency, and accelerate skill development.

---

# Key Findings

* Student skill levels vary significantly across skill categories.
* Meaningful learner segments were identified using clustering.
* Multiple skills exhibit strong learning associations.
* Predictive modeling can estimate future skill proficiency.
* Personalized learning recommendations support targeted improvement.

---

# Business Recommendations

1. Implement personalized learning paths for each learner segment.
2. Prioritize training for skills with the largest learning gaps.
3. Use clustering insights to design customized educational content.
4. Recommend related skills based on association rules.
5. Continuously monitor student progress using predictive analytics.
6. Use AI-driven recommendations to improve learning efficiency and outcomes.

---

# Conclusion

The Skill Gap Analysis System successfully integrates clustering, association rule mining, and predictive modeling to analyze student learning behavior. The solution provides actionable insights, learner segmentation, future skill prediction, and personalized learning recommendations that can enhance educational effectiveness and support student success.
