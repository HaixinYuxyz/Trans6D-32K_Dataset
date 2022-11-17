# Trans6D-32K_Dataset
This is the repository of the dataset and video material for the paper TGF-Net: Sim2Real Transparent Object 6D Pose Estimation Based on Geometric Fusion.

![image](https://github.com/HaixinYuxyz/Trans6D-32K_Dataset/blob/main/Img/dataset_new.jpg)

The proposed dataset contains ten kinds of objects, all of which are common types of objects in households. In order to include as many types of objects as possible, the ten objects include 5 symmetrical objects and 5 asymmetrical objects.

Since the synthetic dataset is made without noise such as motion blur and camera distortion, it is purer than the real dataset. We select 400 images of each object for training, which is large enough to train an accurate 6D pose estimation network. The backgrounds of the 400 images in the train dataset are generated by extracting one frame per ten frames of a video. At the same time, we extract 5000 backgrounds from another completely different video, and use these 5000 backgrounds to randomly generate a test dataset. We generate 2800 images for each object as a test dataset, so the entire dataset contains 32000 images, which we name Trans6D-32K. The test dataset and the train dataset do not have exactly the same background, and using different videos in the train dataset and the test dataset can make the background gap between them larger, so as to verify whether our method can resist the interference of the background by learning geometric features.
