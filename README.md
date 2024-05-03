# A-Comparative-Study-On-Facial-Emotion-Recognition

Abstract— Facial emotion recognition (FER) has garnered significant attention due to its applications in human-computer interaction, healthcare, psychology, and entertainment. This research addresses critical gaps in FER, including the lack of publicly released code, lack of standardized platforms where each researcher is having his/her own hardware and software specification, limited used of evaluation metrics in evaluating the performance of algorithms, and limited of comparison scope among algorithms. In this study, these datasets: CK, FER aligned, FER aligned + CK, RAF-DB, and AffectNet are used in the experiment. We suggest the use of cloud-based platform, i.e. Kaggle as the standardized platform and released the code through GitHub. Different techniques such as image pre-processing and transfer learning are applied to evaluate the impact on the classification results of the selected deep learning models. We include classification accuracy, confusion metrics and recall for the evaluation metrics. As a results, DenseNet121 with pre-trained weights stands out for its high accuracy across datasets, especially in capturing subtle expressions. This study is not only filling in existing gaps but also paving the way for more exact, reliable, and trustworthy FER applications that contribute to broader social benefits and advancements in this area.

# Datasets

The research focuses on a comparative study of Facial Emotion Recognition (FER) using diverse datasets: CK dataset, FER aligned dataset, a combination of FER aligned with CK dataset, RAF-DB dataset, and AffectNet dataset. The CK and FER aligned datasets offer well-defined emotion categories and sufficient images, while their combination further enhances coverage. The RGB format and diverse emotions in the RAF-DB dataset and the high-resolution images in AffectNet provide unique strengths. The multiple datasets allow researchers to choose based on specific requirements like standardized expressions, diverse emotions, RGB analysis, or high-resolution imaging, facilitating advancements in FER. TABLE below shows the details of datasets used in the experiment where the number of data samples for each emotion is reported under ‘Emotions’ and the dimensions and number of channels (i.e. 3 is for RGB and 1 is for grayscale) is reported under ‘Input Shape’.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/44632d6e-1758-42aa-b305-fb3eebf396f3)


For access to valuable data, it’s recommended that everyone download the dataset available at 👇https://drive.google.com/drive/folders/1S5UIGynMALlFpxdh4qJQkY1jln6shYb3?usp=drive_link 

# DenseNet's Accuracy

The TABLE below shows the results of DenseNet model, which included both pre-trained and custom network variants, revealed that the pre-trained DenseNet121 models were superior in terms of accuracy and transferability across varying datasets.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/1fa2342c-1852-43ba-ae6c-50446e3ed5c5)

# ResNet's Accuracy

TABLE below shows the final accuracy of various ResNet model on different datasets, considering both the Custom ResNet and Pre-trained ResNet50 variants as well as their training and testing accuracies.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/ff5baabf-d7a7-4f58-88ef-674b711a2139)


# InceptionNet's Accuracy

TABLE below shows the final accuracy of various InceptionNet model on different datasets, considering both the Custom InceptionNet and Pre-trained Inception V3 variants, along with their respective training and testing accuracies.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/3c9fd3eb-0e6c-4f3d-aebd-7c31a7be9674)

# XceptionNet's Accuracy

TABLE below shows the final accuracy of various XceptionNet model on different datasets, considering both the Custom XceptionNet and Pre-trained Xception variants, along with their respective training and testing accuracies.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/24c57d66-60f0-43da-957d-8894b396e38e)

# Proposed Method's Accuracy

TABLE below is a summary of the performance of the proposed methods across different datasets. Proposed Custom ResNet and Custom XceptionNet achieved 100% accuracy on the CK dataset. For the FER aligned dataset, the DenseNet121 model, that was pre-trained came up with an accuracy of 0.7318, improving to 0.7763 when combined with the CK dataset. The pre-trained DenseNet121 model obtained 0.8488 accuracy on RAF-DB and 0.6304 on AffectNet. These results showed that the proposed method had the highest accuracy among the others, which showed that it was effective in face emotion recognition tasks across different datasets.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/4316f771-ba1a-4390-bbed-a85ecdd2327d)

