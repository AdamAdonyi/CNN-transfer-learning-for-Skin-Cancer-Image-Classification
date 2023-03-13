# SkinCancerPrediction

Based on [publickly available](https://www.kaggle.com/datasets/kylegraupe/skin-cancer-binary-classification-dataset), already categorised data, such as **Cancer** or **Non_Cancer**, I tested 4 different pre-train models, in order to be able to predict category of unseed pictures (isolated from the original dataset)


# Dataset
The [Skin Cancer Binary Classification Dataset](https://www.kaggle.com/datasets/kylegraupe/skin-cancer-binary-classification-dataset) contains several pictures with different sizes such as the following ones (one of it Non_Cancer - guess which one):

<img src="https://github.com/AdamAdonyi/SkinCancerPrediction/blob/main/1051-3(94).jpg" width="50%" height="50%"/> |
<img src="https://github.com/AdamAdonyi/SkinCancerPrediction/blob/main/669-3.JPG" width="45%" height="45%"/>

# Models

Using [learning transfer](https://www.spiceworks.com/tech/artificial-intelligence/articles/articles-what-is-transfer-learning/) from [keras](https://keras.io/api/applications/), we have many option to start with pre-trained models. My top 4, what I wanted to test were; resnet18, [resnet50](https://keras.io/api/applications/resnet/#resnet50-function), [resnet152](https://keras.io/api/applications/resnet/#resnet152-function), and [vgg16](https://keras.io/api/applications/vgg/#vgg16-function).

# Method

Data set was loaded as "train_data" containing two folders; **Non_Cancer** (199 pictures) and **Cancer** (79 pictures) and used to introduce to the model. Fine tuning always happened **3** times. In order to test the model with unseen pictures, **Non_Cancer** (5 pictures) and **Cancer**(5 pictures) were isolated and renamed ("c" means cancer meanwhile "nc" means non_cancer in the names therefore we can track them
