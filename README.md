# A-Comparative-Study-On-Facial-Emotion-Recognition

Abstract— Facial emotion recognition (FER) has garnered significant attention due to its applications in human-computer interaction, healthcare, psychology, and entertainment. This research addresses critical gaps in FER, including the lack of standardized platforms, uniform evaluation metrics, and comprehensive algorithm comparisons. The research includes improving the FER through using Kaggle and GitHub platforms. With Kaggle's standardized platform, it will be possible to run machine learning algorithms in the same running environment for researchers, ensuring consistent conditions for algorithm comparisons. Utilizing GitHub as the primary platform, researchers will access a centralized data repository housing diverse datasets and associated codebases, facilitating fair and accurate algorithm evaluations. Moreover, the research also introduces uniform evaluation metrics to enhance algorithm comparisons, encouraging consistency and reliability. By utilizing a variety of datasets such as CK, FER aligned, FER aligned + CK, RAF-DB, and AffectNet, the study conducts a detailed assessment. Outcomes show that DenseNet121 with pre-trained weights achieved high accuracies especially: 0.7318 on the FER aligned, 0.7763 on FER aligned + CK, 0.8488 on RAF-DB, and 0.6304 on AffectNet datasets. The custom ResNet model and the custom XceptionNet model designed for CK dataset yielded 100% accuracy, demonstrating the framework's potential in improving the FER technology for more efficient and accurate emotion recognition systems.

# Datasets

The research focuses on a comparative study of Facial Emotion Recognition (FER) using diverse datasets: CK dataset, FER aligned dataset, a combination of FER aligned with CK dataset, RAF-DB dataset, and AffectNet dataset. The CK and FER aligned datasets offer well-defined emotion categories and sufficient images, while their combination further enhances coverage. The RGB format and diverse emotions in the RAF-DB dataset and the high-resolution images in AffectNet provide unique strengths. The multiple datasets allow researchers to choose based on specific requirements like standardized expressions, diverse emotions, RGB analysis, or high-resolution imaging, facilitating advancements in FER. TABLE below shows the details of datasets used in the experiment where the number of data samples for each emotion is reported under ‘Emotions’ and the dimensions and number of channels (i.e. 3 is for RGB and 1 is for grayscale) is reported under ‘Input Shape’.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/ecfff105-a854-4714-af7f-0e1e2a4f38e2)

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

