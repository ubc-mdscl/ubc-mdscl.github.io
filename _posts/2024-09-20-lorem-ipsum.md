---
layout: post
title: Airfield Hazards: Bird Tracking at Airports
subtitle: Student Capstone Project
cover-img: /assets/img/airport.png
thumbnail-img: /assets/img/airport-thumb.png
share-img: /assets/img/airport-thumb.png
---

Bird-aircraft strikes pose a significant safety hazard to aircraft, pilots and passengers. In the 2020 alone, the projected cost of wildlife strikes, such as birds, totaled $124 million USD.

In order to address this hazard, Illuminex AI, an organization that automates inspection tasks for unprecedented safety and productivity, worked with a group of UBC Master of Data Science (MDS) Vancouver students to develop a robust object detection pipeline to identify birds in images around airfields in real-time. The pipeline developed takes an image as an input, and outputs the bounding boxes of the birds in the image, as it defines the coordinates of the object.

While there are radar solutions for bird detection, the AI solution developed by the students presented a more cost-effective alternative, which is especially important for smaller airports.

The students’ data contained 98,324 images but only 15 percent were sampled, resulting in only 14,669 images used for training and testing purposes.

Images were taken during daylight hours at a single airport across an entire year. As well, the images had various sizes taken by different cameras. Most images had at least one bird where the bounding boxes were manually, carefully annotated. Birds smaller than 10 pixels were labeled as "small birds". Small birds were usually far away from the camera and airport. This wasn’t too much of a concern for Illuminex as such birds pose a reduced threat to aircraft.

Each sample image contained at least one large bird and the students had a goal to identify birds near the airport. In addition, the group randomly took some images without large birds as negative samples.

During pre-processing, the students re-sized all the images to a uniform resolution of 1080x1920. The second step was data augmentation, where they randomly added planes to ten percent of the images in their dataset to better train their model and avoid false positives. The group also increased the contrast ratio as a third step. This adjustment would simplify the classification between objects and the bright sky.

The students looked at several models including YOLOv8, Faster R-CNN and RetinaNet. When compared to the Ground Truth (the expected result), both RetinaNet and YOLOv8 performed.

But RetinaNet outperformed YOLOv8 in certain scenarios, particularly with small object detection. The RetinaNet model also made duplicate predictions for the same bird but this was resolved by adjusting the nms_threshold parameter, which controls the Non-Maximum Suppression (NMS) process. NMS helps reduce overlapping bounding boxes for the same objects.

The students concluded that their preprocessing steps significantly improved the performance of their model. They were also able to demonstrate the importance of fine-tuning these pre-trained models on their dataset.

Another experiment involved comparing results from filtered label data, where small birds were removed, against unfiltered label data.

One of the challenges the students faced included no other objects were labeled in the images. This issue was addressed by synthetically adding airplanes to the data as part of the preprocessing pipeline.

In the future, students would like to carry out more robust experiments, use the sequential nature of the data, find a solution for night time images, discuss with Illuminex AI about concrete implementation of an alert system, and make the model more robust to different camera positions.
