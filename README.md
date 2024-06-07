# A-Comparative-Study-on-Facial-Emotion-Recognition-by-using-Deep-Learning

Abstract— Facial emotion recognition (FER) has garnered significant attention due to its applications in human-computer interaction, healthcare, psychology, and entertainment. Deep learning algorithms have been widely applied and improve the performance of FER. However, some critical gaps in FER, including the lack of standardized comparative platforms, limited used of evaluation metrics may have hinder the comprehensive understanding of various deep learning algorithms in FER. This study proposed some useful guidelines which include a standardized platform, more evaluation metrics and explored the impact of transfer learning and input size on FER. These datasets: CK, FER aligned, FER aligned + CK, RAF-DB, and AffectNet are used in the experiment. The research used the cloud-based platform, i.e. Kaggle as the standardized platform and the code was released through GitHub. Through the suggested guidelines for evaluation, some interesting insights such as the performance of each different emotion for each dataset and each deep learning algorithm, the impact of different input sizes and transfer learning are revealed.

In this study, the contribution is as below: 
1.	A cloud-based platform that can be easily used by all the other researchers as a standard platform and the release of code for benchmarking purposes.
2.	More evaluation metrics besides classification accuracy where this includes the recall.
3.	The impact of transfer learning and input dimensions are explored in this comparative study. 


# Datasets

The research focuses on a comparative study of Facial Emotion Recognition (FER) using diverse datasets: CK dataset, FER aligned dataset, a combination of FER aligned with CK dataset, RAF-DB dataset, and AffectNet dataset. The CK and FER aligned datasets offer well-defined emotion categories and sufficient images, while their combination further enhances coverage. The RGB format and diverse emotions in the RAF-DB dataset and the high-resolution images in AffectNet provide unique strengths. The multiple datasets allow researchers to choose based on specific requirements like standardized expressions, diverse emotions, RGB analysis, or high-resolution imaging, facilitating advancements in FER. TABLE below shows the details of datasets used in the experiment where the number of data samples for each emotion is reported under ‘Emotions’ and the dimensions and number of channels (i.e. 3 is for RGB and 1 is for grayscale) is reported under ‘Input Shape’.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/8d52871d-30f0-4b94-ab3c-0f4ffabbc95c)


For access to valuable data, it’s recommended that everyone download the dataset. The dataset is available at 👇https://drive.google.com/drive/folders/1S5UIGynMALlFpxdh4qJQkY1jln6shYb3?usp=drive_link 

# Prcoess Flow

Some of the terminologies used in this study are: models with pre-defined input dimensions are named as custom models (the verification of input size is reported in Section IV.B); for models with transfer learning, it is named as pre-trained models. Pre-processing techniques are applied on all the input data for all the deep learning models in this study. However, for pre-trained model, grayscale transformation is not applied.

FIGURE below the process flow of the custom model for FER. The flow of the custom model encompasses multiple stages, namely input size customization, load dataset, image preprocessing, separate train and test set, custom model, model setup, and evaluation. 

![Process flow of the custom model](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/12062557-4c68-4a27-b4bd-fdde93577349)

FIGURE below depicts the process flow of the pre-trained model for FER. The flow of the pre-trained  model includes load dataset, image preprocessing, separate train and test set, pre-trained model, build model on top of pre-trained model, train the top layer, fine-tuning the entire model, and evaluation.

![Process flow of the pre-trained model](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/e6df8140-6912-4b21-bf74-079046ea2e0e)


# Accuracy of all models

The TABLE below shows the accuracy results of various deep learning algorithms on different datasets. For pre-trained models, input size with the highest testing accuracy are selected. The input size was listed under the column ‘Models’. For CK dataset, Custom ResNet50 and Custom Xception achieved 100% testing accuracy. Pre-trained DenseNet121 yielded a higher testing accuracy of 0.7318, demonstrating its ability to capture complex features for emotion recognition in FER aligned. In the FER aligned + CK dataset, Pre-trained DenseNet121 again achieved the highest testing accuracy, i.e. 0.7763. The strength of DenseNet121 is also shown in RAF-DB dataset, where the image input was maintained in RGB mode. Pre-trained DenseNet121 achieved 0.8488 testing accuracy. Lastly, on the AffectNet dataset, Pre-trained DenseNet121 again scored the highest with 0.6304 testing accuracy, highlighting its capability to recognize subtle facial expressions. 

![Accuracy of All Models](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/8f6554c1-5f91-486c-8524-1e4000727bf0)

# Average Performance of Deep Learning Models

The GRAPH IMAGE below presents and compares the classification strength between custom models and pre-trained models.  Among all the models, DenseNet121 has the highest classification accuracy, i.e. 0.7908. The dense connectivity in DenseNet121 and feature reuse are well contributed to its efficient learning, making it suitable for various datasets targeting the FER. In terms of custom model, ResNet50 has the best achievement among all the compared models, i.e. 0.7651.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/4d651ba4-3f3c-4b97-b7c6-97728bca7d5d)






# DenseNet's Accuracy

The TABLE below shows the results of DenseNet model, which included both pre-trained and custom network variants, revealed that the pre-trained DenseNet121 models were superior in terms of accuracy and transferability across varying datasets.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/b87a1d22-3948-48e9-9b3c-dd9a9f8e45a0)


# ResNet's Accuracy

TABLE below shows the final accuracy of various ResNet model on different datasets, considering both the Custom ResNet and Pre-trained ResNet50 variants as well as their training and testing accuracies.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/002f6c5a-5a68-48cb-a13a-354c0dae986e)


# InceptionNet's Accuracy

TABLE below shows the final accuracy of various InceptionNet model on different datasets, considering both the Custom InceptionNet and Pre-trained Inception V3 variants, along with their respective training and testing accuracies.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/b9e6d707-c19d-4298-9072-fd2617da6e65)


# XceptionNet's Accuracy

TABLE below shows the final accuracy of various XceptionNet model on different datasets, considering both the Custom XceptionNet and Pre-trained Xception variants, along with their respective training and testing accuracies.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/56e8fc1a-93d9-478d-bd1d-7379ae4f5197)


# Proposed Method's Accuracy

TABLE below is a summary of the performance of the proposed methods across different datasets. Proposed Custom ResNet and Custom XceptionNet achieved 100% accuracy on the CK dataset. For the FER aligned dataset, the DenseNet121 model, that was pre-trained came up with an accuracy of 0.7318, improving to 0.7763 when combined with the CK dataset. The pre-trained DenseNet121 model obtained 0.8488 accuracy on RAF-DB and 0.6304 on AffectNet.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/06e1d6b4-1186-4c30-be62-cfb0e61bb8ca)


# Summary of the Result of Comparison Among All Models

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/721c44ef-aef5-4b1a-bb7d-cc93263ac6e0)


The FIGURE above the testing accuracy of all models in graph version. Ultimately, it can be summarized that the model of DenseNet with Pre-trained (DenseNet121) is highly accurate and generalizes well across different datasets, demonstrating robustness, feature extraction, and generalization ability. The practice of using pre-trained models usually results in a higher testing accuracy and more efficient performances, and this can be particularly useful in tasks such as emotion classification where knowledge provided by the pre-existing models forms the backbone of the model training and inference. In this respect, the DenseNet model with Pre-trained (DenseNet121) outperforms the other ones and provides high accuracy across various emotions recognition tasks. Hence, DenseNet121 proves to be an effective model on many different datasets because of its architecture as well as its training methods. This dense connectivity pattern involves feature reuse and enables the propagation of information across the network, introducing efficient learning and representation of complicated patterns. Also, the utilization for transfer learning of pre-trained weights increases the model’s generalization ability by using knowledge from large-scale datasets. Such integration of architectural design, feature reuse, and transfer learning is responsible for the overall robustness and high accuracy of this network across distinct dataset setups. 
