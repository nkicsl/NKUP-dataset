# 1.NKUP Dataset Description

Person re-identification(re-ID) has drawn attention significantly in the computer vision society due to its application and research significance. It aims to retrieve a person of interest across different camera views. However, there are still several factors that hinder the applications of person re-ID. In fact, most common datasets either assume that pedestrians do not change their clothing across different camera views or are taken under constrained environments. Those constraints simplify the person re-ID task and contribute to early development of person re-ID, yet a person has a great possibility to change clothes in real life. To facilitate the research towards conquering those issues, we mainly introduce a new benchmark dataset named “NKUP”. To the best of our knowledge, this dataset is currently the most diverse for person re-identification, varying according to viewpoints, lighting, resolutions, human pose, seasons, backgrounds, and clothes especially.  
The NKUP dataset is collected with fifteen cameras, including eight indoor cameras and seven outdoor cameras, in the open environment of Nankai University. Then, we crop pedestrain images by pedestrian detectors from the surveillance videos, obtaining the motion sequence of each pedestrian and a total of over 200,000 bounding boxes with IDs. After that, we selected one image per 25 frames from the continuous pedestrian images to get the image-based dataset. As a result, we get 5,336 training images of 40 identities, 332 query images 4,070 gallery images of 67 identities. On average, each person in the dataset has 2.2 kinds of clothes and 2.6 kinds of clothes except for the distractor.  

# 2.NKUP+ Dataset Description
The Re-ID with cross-appearance in long-term period has become one of the latest directions for ReID. Because the cross-appearance scenes are also common in real world, and it is unreliable to conduct Re-ID with only the appearance features in such cases. Models trained on the dataset containing cross-appearance images can pay attention to more robust features in the process of feature extraction. In recent years, some researchers have proposed cross-appearance datasets. However, due to personnel and time constraints, the existing datasets probably have several disadvantages: 1) The sizes of the datasets are small because it is not easy to organize a large number of people for a long time; 2) Some works took other approaches to collect images, such as celebrity street shots, movies and TV shows, and those datasets are trapped in domain adaptation problem; 3) The source videos were collected in a short time interval, and there are no obvious appearance changes, which is inconsistent with the real scenarios such as capturing the suspects who were skillful at anti-tracking and changed their clothing dramatically.

Therefore, we proposed a long-term and publicly available person re-ID dataset containing images of multiple appearances named NKUP+. The surveillance videos are collected from 29 indoor and outdoor cameras of Nankai University, and there are more than 40,000 pedestrian images in the dataset. For each person, we provide a variety of images from multiple cameras and perspectives. To be able to fully evaluate the retrieval performance of the model, the test set is devided into several subsets according to different appearances of the person. The images with the same appearance as the query constitute the same-appearance gallery, while the images with a time interval of more than three months constitute dramatic cross-appearance gallery, otherwise the images constitute moderate cross-appearance gallery.


# 2.Download

Please download the NKUP dataset using the links below: [Baidu Yun](https://pan.baidu.com/s/1f4b-tpRZYIwiUTbmIDNPRQ)(code:ik5s) or [Google Drive](https://drive.google.com/drive/folders/1xVJylT2sa2KqWu9kVfi6r10TOXAlR8wp?usp=sharing)


And you can download the NKUP+ dataset using the links below: [Baidu Yun](https://pan.baidu.com/s/1e3UHs_eZddyuRlJHU3oUHg?pwd=cn63)(code:cn63). If you have any questions about downloading the dataset, please contact us by sending email to aics@nankai.edu.cn.

# 3.Content

The NKUP folder contains three files:  
   - "bounding_box_train.zip" file. This file contains 5336 images for training.  
   - "bounding_box_test.zip" file. This file contains 4070 images for testing and we retrieve a query from this image pool.  
   - "query.zip" file. It contains 332 query images. Each of them is not collected on the same day as those of the same person in the "bounding_box_test" file. In      other words, their clothes are different.  


The NKUP+ folder contains two files:
   - "bounding_box_train.zip" file. This file contains 22590 images for training.  
   - "bounding_box_test.zip" file. This file contains 4 folders including query, same appearance gallery, moderate appearance gallery and dramatic appearance gallery.  

# 4.LICENSE

   - The images and the corresponding annotation results can only be used for ACADEMIC PURPOSES. NO COMERCIAL USE is allowed.  
   - Copyright © College of Computer Science, Nankai University. All rights reserved.  

# 5.Cite

Please cite the following paper if NKUP dataset helps your research:  
Wang K, Ma Z, Chen S, Yang J, Zhou K, Li T. A benchmark for clothes variation in person re-identification. Int J Intell Syst. 2020;1-18. https://doi.org/10.1002/int.22276

Please cite the following paper if NKUP+ dataset helps your research: 
Mengmeng Liu, Zhi Ma, Tao Li, Yanfeng Jiang, and Kai Wang. 2022. Long-Term Person Re-identification with Dramatic Appearance Change: Algorithm and Benchmark. In Proceedings of the 30th ACM International Conference on Multimedia (MM ’22), October 10–14, 2022, Lisboa, Portugal. ACM,New York, NY, USA, 10 pages. https://doi.org/10.1145/3503161.3548327
