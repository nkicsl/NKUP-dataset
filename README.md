# 1.NKUP Dataset Description

Person re-identification(re-ID) has drawn attention significantly in the computer vision society due to its application and research significance. It aims to retrieve a person of interest across different camera views. However, there are still several factors that hinder the applications of person re-ID. In fact, most common datasets either assume that pedestrians do not change their clothing across different camera views or are taken under constrained environments. Those constraints simplify the person re-ID task and contribute to early development of person re-ID, yet a person has a great possibility to change clothes in real life. To facilitate the research towards conquering those issues, we mainly introduce a new benchmark dataset named “NKUP”. To the best of our knowledge, this dataset is currently the most diverse for person re-identification, varying according to viewpoints, lighting, resolutions, human pose, seasons, backgrounds, and clothes especially.  
The NKUP dataset is collected with fifteen cameras, including eight indoor cameras and seven outdoor cameras, in the open environment of Nankai University. Then, we crop pedestrain images by pedestrian detectors from the surveillance videos, obtaining the motion sequence of each pedestrian and a total of over 200,000 bounding boxes with IDs. After that, we selected one image per 25 frames from the continuous pedestrian images to get the image-based dataset. As a result, we get 5,336 training images of 40 identities, 332 query images 4,070 gallery images of 67 identities. On average, each person in the dataset has 2.2 kinds of clothes and 2.6 kinds of clothes except for the distractor.  

# 2.Download

Please download the dataset using the links below: [Baidu Yun](https://pan.baidu.com/s/1f4b-tpRZYIwiUTbmIDNPRQ)(code:ik5s)

# 3.Content

The folder contains three files:  
   - "bounding_box_train.zip" file. This file contains 5336 images for training.  
   - "bounding_box_test.zip" file. This file contains 4070 images for testing and we retrieve a query from this image pool.  
   - "query.zip" file. It contains 332 query images. Each of them is not collected on the same day as those of the same person in the "bounding_box_test" file. In      other words, their clothes are different.  

# 4.LICENSE

   - The images and the corresponding annotation results can only be used for ACADEMIC PURPOSES. NO COMERCIAL USE is allowed.  
   - Copyright © College of Computer Science, Nankai University. All rights reserved.  

# 5.Cite

Please cite the following paper if this dataset helps your research:  
Wang K, Ma Z, Chen S, Yang J, Zhou K, Li T. A benchmark for clothes variation in person re-identification. Int J Intell Syst.2020;0-0. https://doi.org/10.1002/int.22276

