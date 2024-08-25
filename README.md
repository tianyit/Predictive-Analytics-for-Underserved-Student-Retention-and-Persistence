# Predictive Analytics for Underserved Student Retention and Persistence
Non-returning students represent a lost investment for all parties involved: the students themselves, the institutions, and supporting organizations. 

Previous studies have identified predictors of retention to include academic performance indicators (e.g., high school GPA, SAT/ACT scores, college GPA), demographic factors (age, gender, ethnicity), and socio-economic status (SES). These factors, along with institutional characteristics such as the type of institution (public/private, 4-year/2-year), play a significant role in student retention and persistence.

This study utilizes a machine learning framework to predict student retention and persistence
for student from underserved communities, using a combination of institutional and individual student data. This study aims to provide actionable insights that can help supporting organizations better support student populations by paying more attention to the students at more risk of dropping out of the institution.

The research addresses the following questions:
1. Which features are most predictive of student retention and persistence, respectively?
Retention: First-generation status, age, and household composition emerged as significant
predictors, with first-generation students showing a higher likelihood of dropping out. Older
students and those from two-parent households were less likely to drop out, likely due to
more stable support systems and matured life perspectives.
Persistence: Similar factors impact persistence, but the increased magnitude of coefficients
for first-generation status indicates greater challenges in continuity at the initial institution, possibly due to inadequate institutional fit or support.

2. How accurately can we predict a student’s likelihood of discontinuing their studies using
information from a combination of the institutional data and student data?
The use of Gradient Boosting has shown that it is possible to achieve substantial accuracy in
predicting student persistence outcomes, with 86.13% AUC-ROC scores indicating effective
discriminative ability between students who are likely to continue their studies versus those
who might drop out. For retention, SVM, with AUC-ROC score 71.41%, showed improved generalization
capabilities after model adjustments, making it suitable due to its robustness against
overfitting.

3. How do the factors influencing student retention compare with those affecting student
persistence, and what are the implications for predictive modeling in educational settings?
Retention involves predicting whether students return to the same institution. This can often
mean dealing with a narrower set of variables that influence this decision—factors directly
related to a specific institution such as campus environment, academic programs, and student
services. If the model is trained on detailed but institution-specific data, it might perform
exceptionally well on training data but fail to generalize beyond that because it learns too
deeply the nuances of the specific training dataset's environment. To achieve high accuracy, retention models might become complex as they try to capture all
institutional nuances and student interactions within a single institution. This complexity can
lead to overfitting when the model becomes too tailored to the training data, capturing noise
rather than the underlying pattern.
Persistence, on the other hand, reflects a broader concept—whether students continue their
education at any institution. Therefore, the features influencing persistence are likely more
varied and less specific to a particular institution's characteristics. This can lead to a model
that generalizes better because it learns from a broader base of factors that affect students' decisions to continue education anywhere.
