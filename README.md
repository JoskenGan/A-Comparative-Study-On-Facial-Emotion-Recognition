![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/52b0630f-909c-414c-ab69-efc5f32662c4)# A-Comparative-Study-on-Facial-Emotion-Recognition-by-using-Deep-Learning

Abstract— Facial emotion recognition (FER) has garnered significant attention due to its applications in human-computer interaction, healthcare, psychology, and entertainment. This research addresses critical gaps in FER, including the lack of publicly released code, lack of standardized platforms where each researcher is having his/her own hardware and software specification, limited used of evaluation metrics in evaluating the performance of algorithms, and limited of comparison scope among algorithms. In this study, these datasets: CK, FER aligned, FER aligned + CK, RAF-DB, and AffectNet are used in the experiment. We suggest the use of cloud-based platform, i.e. Kaggle as the standardized platform and released the code through GitHub. Different techniques such as image pre-processing and transfer learning are applied to evaluate the impact on the classification results of the selected deep learning models. We include classification accuracy, confusion metrics and recall for the evaluation metrics. As a results, DenseNet121 with pre-trained weights stands out for its high accuracy across datasets, especially in capturing subtle expressions. This study is not only filling in existing gaps but also paving the way for more exact, reliable, and trustworthy FER applications that contribute to broader social benefits and advancements in this area.

In this study, the contribution is as below: 
1.	A cloud-based platform through Kaggle that is accessible by everyone is used as a standard platform. This ease the challenge of different specification in hardware and software.
2.	The code on how we compare each algorithm is released through GitHub: https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition 
3.	We include few evaluation metrics, i.e. confusion metrics, classification accuracy and recall. 
4.	The scope of experiments is expanded by including pre-processing techniques, transfer learning and the impact of input dimensions to explore insights the strengths and weaknesses of each algorithm in this comparative study. This helps researchers and developers make informed choices of most suitable algorithm for facial emotion recognition.


# Datasets

The research focuses on a comparative study of Facial Emotion Recognition (FER) using diverse datasets: CK dataset, FER aligned dataset, a combination of FER aligned with CK dataset, RAF-DB dataset, and AffectNet dataset. The CK and FER aligned datasets offer well-defined emotion categories and sufficient images, while their combination further enhances coverage. The RGB format and diverse emotions in the RAF-DB dataset and the high-resolution images in AffectNet provide unique strengths. The multiple datasets allow researchers to choose based on specific requirements like standardized expressions, diverse emotions, RGB analysis, or high-resolution imaging, facilitating advancements in FER. TABLE below shows the details of datasets used in the experiment where the number of data samples for each emotion is reported under ‘Emotions’ and the dimensions and number of channels (i.e. 3 is for RGB and 1 is for grayscale) is reported under ‘Input Shape’.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/8d52871d-30f0-4b94-ab3c-0f4ffabbc95c)


For access to valuable data, it’s recommended that everyone download the dataset. The dataset is available at 👇https://drive.google.com/drive/folders/1S5UIGynMALlFpxdh4qJQkY1jln6shYb3?usp=drive_link 

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

TABLE below is a summary of the performance of the proposed methods across different datasets. Proposed Custom ResNet and Custom XceptionNet achieved 100% accuracy on the CK dataset. For the FER aligned dataset, the DenseNet121 model, that was pre-trained came up with an accuracy of 0.7318, improving to 0.7763 when combined with the CK dataset. The pre-trained DenseNet121 model obtained 0.8488 accuracy on RAF-DB and 0.6304 on AffectNet. These results showed that the proposed method had the highest accuracy among the others, which showed that it was effective in face emotion recognition tasks across different datasets.

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/06e1d6b4-1186-4c30-be62-cfb0e61bb8ca)


# Summary of the Result of Comparison Among All Models

![image](https://github.com/JoskenGan/A-Comparative-Study-On-Facial-Emotion-Recognition/assets/168083511/721c44ef-aef5-4b1a-bb7d-cc93263ac6e0)


The figure above the testing accuracy of all models in graph version. Ultimately, it can be summarized that the model of DenseNet with Pre-trained (DenseNet121) is highly accurate and generalizes well across different datasets, demonstrating robustness, feature extraction, and generalization ability. The practice of using pre-trained models usually results in a higher testing accuracy and more efficient performances, and this can be particularly useful in tasks such as emotion classification where knowledge provided by the pre-existing models forms the backbone of the model training and inference. In this respect, the DenseNet model with Pre-trained (DenseNet121) outperforms the other ones and provides high accuracy across various emotions recognition tasks. Hence, DenseNet121 proves to be an effective model on many different datasets because of its architecture as well as its training methods. This dense connectivity pattern involves feature reuse and enables the propagation of information across the network, introducing efficient learning and representation of complicated patterns. Also, the utilization for transfer learning of pre-trained weights increases the model’s generalization ability by using knowledge from large-scale datasets. Such integration of architectural design, feature reuse, and transfer learning is responsible for the overall robustness and high accuracy of this network across distinct dataset setups. 
