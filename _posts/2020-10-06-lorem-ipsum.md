---
layout: post
title: Mineral Occurrence Text Extractor
subtitle: Student Capstone Project
cover-img: /assets/img/mineral-extractor.jpg
thumbnail-img: /assets/img/mineral-extractor-thumb.png
share-img: /assets/img/mineral-extractor-thumb.png
---

Minerva Intelligence is an artificial intelligence company that provides structured knowledge in earth science domains like mining and natural hazards.

Minerva partnered with students from the Master of Data Science in Computational Linguistics program to extract information from MINFILE, a British Columbia government mineral occurrences database.

A mineral occurrence is where useful minerals have been found and there is a potential for a mine to be developed. This information can be very valuable to geologists searching for new mines.

The team downloaded a little over 15,000 reports from the government database. These reports were broken down into different fields such as “Commodities” that lists the commodity found at a mineral occurrence and the “Capsule Geology” which is the written portion of the report that contains a reference to one or more commodities, as well as other information that could be harvested.

For example, one report would list ‘lead’ in the Commodities field meaning that ‘lead’ is a commodity that was found at that particular mineral occurrence. In the Capsule Geology field, ‘lead’ should have been mentioned somewhere within the text, as well as, possibly, the rock type which hosted it, such as “granite”.

The focus of the capstone project was to use the “Capsule Geology” text to fill in the “Commodities” field with commodities that may have been overlooked, as well as other fields such as “Host Rock”.

The team developed a way to extract relevant sentences that contain terms that can be found in the commodity field and after some more processing they fed the data into the commodity model and the model's output would be true or false; true meaning that the term is a commodity and false meaning the term is not.

Additionally, the project involved expanding a lexicon of minerals using morphology.

For example, the Capsule Geology may note a mineral that contains lead and the purpose of the lexicon was to build the connection between said mineral and lead.

The information that the team extracted can be added to Minerva's knowledge base and ultimately help make their AI system more robust.
