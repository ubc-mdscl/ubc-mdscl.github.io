---
layout: post
title: Why do Judges Allow or Deny Eviction Orders in Ontario's Residential Tenancy Board?
subtitle: Student Capstone Project
cover-img: /assets/img/law-capstone-project.png
thumbnail-img: /assets/img/law-capstone-project-thumb.png
share-img: /assets/img/law-capstone-project-thumb.png
---

The University of Toronto’s Future of Law Lab worked with two groups of Master of Data Science Computational Linguistics students to help answer the following question: Why do judges allow or deny eviction orders in Ontario's Residential Tenancy Board?

The first group were tasked with doing automatic information extraction from online case files 

The goal of this project was to develop a system that can predict the outcome of future cases within Ontario in the domain of housing law.

To reach this goal, the students broke it down to two main tasks: data mining (extracting information from the cases) and case prediction.

The team were presented with 700 manually annotated files where the information extracted were manually verified.

To extract information, they used a combination of rule-based methods and machine learning models. One of the challenges the team faced was there was no pre-existing way to automatically get all of the text from cases, so they had to develop their own method. The data mining team then built a framework that included a hybrid approach of rule-based extraction algorithms and Large Language Models to achieve this. However, to develop and further improve these models, the team also developed a web app which would facilitate and streamline the manual annotation of more case files in the future. This helps to improve both the extraction system and the quality of the predictions made by the prediction team’s model.

This would then be converted into a database of annotated cases which is built upon the initial 700 cases that were provided to the team. As the number of correctly annotated cases increases, so should the quality of the prediction model’s predictions in regards to future cases. This model is designed to specifically determine which cases are more likely to succeed for the tenant at trial, help the client understand their own situation, and help lawyers understand what the judges are looking for, such as which factors of a case may be contribute most to the outcome of a case.

As with the first group, the prediction model team’s data contained 700 human-annotated cases. These cases were a sample of all cases from 2017-2020 based on the record from Canadian Legal Information Institute (CanLII). The data was annotated by different first/second year law students from 2020 to 2021. 

After cleaning the data, the team ended up with 696 cases remaining (some had to be removed due to reasons such as insufficient data) and 47 features, such as location of the landlord tenant board wherein the case was heard, the member adjudicating the decision, and the outcome of the case.

Since the students were doing supervised machine learning, they split 80% of the data into a training subset and 20% of the data into a testing subset. 

The team tried four models but determined that the non-linear Light GBM had around 81% accuracy when evaluated against the test subset. However, the team’s final product used a technique called Ensembling, which combines multiple predictive models to obtain better performance. Ensembling helped to minimize noise, variances and biases in order to achieve improved accuracy and better generalization to future cases.

Despite the project’s success, the team felt that there was a lot that could be done going forward. This includes improving annotations, updating the machine learning model(s) used, and further developing the annotation web app to best serve annotators
