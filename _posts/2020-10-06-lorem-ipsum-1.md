---
layout: post
title: Analysis of BC Negligence Decisions over 20 years
subtitle: Student Capstone Project
cover-img: /assets/img/bc-decisions.jpg
thumbnail-img: /assets/img/bc-decisions-thumb.png
share-img: /assets/img/bc-decisions-thumb.png
---

UBC’s Peter A. Allard School of Law worked with a group of UBC Master of Data Science in Computational Linguistics (MDS-CL) students to examine a trend in payouts to injured British Columbians. Some members of the legal community specializing in negligence cases have begun to suspect that the overall damage payouts have been steadily increasing in British Columbia Supreme Court since the year 2000—at a level above inflation and disconnected from a central rationale.

The goal of this capstone project was to analyze all negligence cases in the province of British Columbia between 2000 and 2020, in order to determine how damages and contributory negligence have been changing over time.

Negligence is a branch of tort law that deals with the breach of duty to take care and it involves harm caused by carelessness, not intentional harm. Negligence cases may involve damage payments to the plaintiff broken down into specific sub-categories based on the evidence presented and the precedence set for similar cases that have occurred in the past. They also may find the plaintiff partially liable for the damages—which is known as contributory negligence.

The project’s data source came from cases pulled from LexisNexus, a corporation that specializes in computer-assisted legal research. In order to complete a meaningful analysis of the data, important pieces of information such as the damages paid and the percentage that the plaintiff is found liable must be extracted from the case reports.

The students focused on two specific methods to develop a system that pulls out relevant information from the case reports: a rules-based classifier (manually laying out specific patterns that a computer will use to search through large amounts of text data and return the text which matched a pattern) and a statistical classifier (a computer inspects potentially relevant pieces of information and determine the group or class the information belongs to).

Overall, the MDS-CL team discovered that the statistical classification method slightly outperformed their rule-based classification method.

The analysis showed that damage payouts in negligence cases in BC are on a general upward trend since 2000. In terms of contributory negligence, the analysis showed a mean of 38% reduction which was stable over the years.

It can be inferred by the data extracted that the overall upward trend will continue to rise in the near future.
