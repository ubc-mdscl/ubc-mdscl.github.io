---
layout: post
title: Gender Gap Statistics on Adjectival Usage in English
subtitle: Student Data Science Project
cover-img: /assets/img/gendergapstat.jpeg
thumbnail-img: /assets/img/gendergapstat-thumb.png
share-img: /assets/img/gendergapstat-thumb.png
---

A group of UBC Master of Data Science (MDS) Computational Linguistics students (Su Yuan, Lusha Wang, and Lisa Zhang) were inspired by Simon Fraser University’s Gender Gap Tracker and decided for their Advanced Corpus Linguistics course project that they wanted to analyze a large news corpus to uncover the gender gap. In particular, the students wanted to further investigate the adjectives and adverbs used to describe different gender (binary gender classification for practical reasons) in The Globe & Mail news articles.

To begin, the students contacted the SFU Discourse Processing Lab for their annotated data on genders of authors and cited authorities to dig deeper on the descriptors. The students ended up obtaining a large collection of roughly 371,000 English news articles published in 2023 from major Canadian news sources (like CBC, CTV, and The Globe and Mail) from the [SFU Discourse Processing Lab](https://gendergaptracker.research.sfu.ca/). For the purpose of their project, the students concentrated on a sample of 500 articles from The Globe & Mail.

With the 500 articles, the students then employed linguistic annotation techniques, specifically dependency parsing and POS tagging, to identify and extract descriptive words (adjectives and adverbs) that are associated with individuals mentioned within these articles. Those descriptive words were then categorized into five key categories: power-related, appearance-related, behavior-related, competence-related, and emotionality-related.

The students then manually annotated each of the identified descriptors with its corresponding category (e.g., “presidential” as “power-related” and “pretty” as “appearance-related”). The descriptors’ distribution allowed them to identify the differences between binary genders, thus strongly suggesting the presence of underlying gender gap in media language across various semantic domains.

What the students discovered was noticeable gendered patterns in major news articles used to describe individuals. 

For example, men were frequently associated with descriptors of power and status (e.g. “strong” and “presidential”), while women were often described in terms of appearance, behavior, and sometimes trivializing attributes that shows some ingrained bias (e.g. “sexy”, "supportive”, and “ridiculous”). 

From the data, the students can conclude that societal biases are subtly woven into the fabric of news reporting, potentially shaping perceptions and perpetuating inequalities. Recognizing these patterns is the crucial first step in challenging and ultimately changing these linguistic norms.

The end result of the project was the development of a manually-annotated corpus that quantifies gendered descriptor patterns in news articles as well as an accompanying interactive website. The website allows users to visualize descriptor frequency via a word cloud, search specific terms and their gender associations (including author gender), filter descriptors by the established categories (power, appearance, behavior, competence, emotion), access original articles with highlighted terms, and allow users to "red flag" annotations of categories they find problematic or arguable, or descriptors that do not modify an individual.

The students believe their project can offer tangible benefits across various domains. For journalists, their findings and the accompanying website serve as a valuable resource for fostering greater awareness of their own linguistic choices, encouraging a more conscious effort towards equitable and unbiased reporting. Natural Language 

Processing researchers can leverage the annotated dataset and analytical insights to evaluate and refine language generation models, working towards AI that avoids replicating existing societal biases. More broadly, by making these subtle linguistic patterns visible and accessible through their user-friendly website, the students aim to empower media consumers and the general public to critically analyze the language they encounter daily, fostering a deeper understanding of how language can shape our perceptions of gender and promoting more critical engagement with media narratives.
