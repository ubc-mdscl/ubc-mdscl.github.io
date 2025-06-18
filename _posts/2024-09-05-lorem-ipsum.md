---
layout: post
title: Predicting Show vs No Show and Job Success in Construction
subtitle: Student Capstone Project
cover-img: /assets/img/faber.png
thumbnail-img: /assets/img/faber-thumb.png
share-img: /assets/img/faber-thumb.png
---

For Faber Connect, a Vancouver-based organization that helps connect construction companies to construction workers for short or long-term work, a significant operational challenge is the unpredictability of worker attendance and worker quality.

Faber turned to a group of UBC’s Master of Data Science (MDS) Vancouver students to create a data product that predicts worker attendance reliability and performance, and to better understand how to improve worker job success. To this end, the students explored both standard metrics of job success as well as novel proxies.

The team worked with an existing database that contained anonymized information on individual workers, their past interactions on Faber’s platform, as well as details about the projects posted. A significant consideration throughout the project was preventing data leakage such that future data would not bias or influence the performance of predictive models. Thus, after consultation with the partner organization, the students performed extensive data engineering and pre-processing in order to mitigate this issue.

Another major consideration was the interpretability and generalizability of the model. As such, the students strayed away from black-box neural networks and focused instead on using linear and ensemble models.

The team found that a combination of workers’ past performance and supportive company practices contributed to worker job success. Some of the key takeaways that the students found was that better incentives usually resulted in higher attendance and reduced the likelihood of negative performance.

The final data product, hosted on Faber's private GitHub repository, contained the model files for each target variable, the data pipeline, and comprehensive documentation, including a detailed user guide.

Given the tight timeframe of the capstone project period, one major challenge that the students faced was becoming fully familiar with the data, industry norms, and concepts. If they had more time, the group felt they could have come up with more optimal feature engineering.

The next challenge was the data received didn’t fully capture worker behavior. Moreover, since many features in the app were optional, the students were faced with multiple missing values.

For future recommendations, the students recommended that Faber use tools such as natural language processing to extract new rich features to capture more of the nuances in worker behavior. 
