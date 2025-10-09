# Public Report
This document outlines the work completed over the past ten weeks as part of the third module of the project. The focus of this phase was the training of the Convolutional Neural Network, encompassing all steps from exploratory analysis to validation. This is the third of four modules that collectively contribute to the final project deliverable.

## I. Project Description
The project aims to assist users in identifying the colors that suit them best. Leveraging computer vision techniques, the system analyzes a user's appearance and suggests one of twelve predefined color palettes tailored to their features. Users can upload a photo and receive a personalized palette. Additionally, the application includes educational content to help users understand the theory behind personal color analysis and the value of the tool. [1][2]

## II. Artifacts
### 2.1 Exploratory Analysis and Data Preprocessing
The first notebook details the exploratory data analysis (EDA) and preprocessing steps undertaken to prepare the dataset for model training. The exploratory analysis involved examining the distribution of classes and the hair and skin tones to ensure a balanced dataset and identify any potential biases. Data preprocessing steps included resizing images and pixel normalization.

### 2.2 Model Training
The second notebook focuses on the training of the Convolutional Neural Network (CNN) using TensorFlow and Keras. Two approaches were explored: training a model from scratch and utilizing transfer learning with pre-trained models such as VGG16, ResNet50, and EfficientNetB0. The notebook includes details on architecture selection, data splitting and training process. [3][4][5]

### 2.3 Model Improvement
The third notebook aimed to improve the model's performance through hyperparameter tuning and other approaches. One of which was to create a multi-input model that takes into account not only the image but also categorical features such as hair and skin tones. Furthermore, it used a 4-class prediction, then a 12-class prediction with gating based on the 4-class output. This hierarchical approach was intended to enhance classification accuracy by narrowing down the options in a structured manner. All the models were evaluated using metrics such as accuracy, precision, recall, F1-score, and confusion matrices to assess their performance comprehensively.

### 2.4 Model Validation
The fourth notebook was dedicated to validating the final model using a separate validation dataset and analyzing the training process through image techniques. This step is crucial to ensure that the model generalizes well to unseen data and performs reliably in real-world scenarios

#### 2.4.1 Interpretability
To understand the model's decision-making process, interpretability techniques such as Grad-CAM, Occlusion Sensitivity, and Saliency Maps were applied. These methods help visualize which parts of the input images the model focuses on when making predictions, providing insights into its behavior and potential areas for improvement. [6][7][8]

#### Real-World Testing
The model was also tested with real-world images to evaluate its performance in practical scenarios. In this phase, we found that the model struggled with images that had complex backgrounds or poor lighting conditions. This highlighted the need for further refinement and potential data augmentation strategies to enhance robustness.

### 2.5 Model Deployment
The VisionPalette service was containerized using Docker. Then, it was deployed on AWS using an EC2 instance. The model was also uploaded to that same instance. A detailed deployment documentation was created for specifications.

### 2.7 Final Presentation
A final presentation was prepared to showcase to the company the completed module, including a live demonstration of the application. The presentation highlighted the overall process of training the convolutional model, the challenges faced, and the solutions implemented, providing an overview of the work accomplished in this module.

## III. Conclusion
This module successfully delivered a functional and integrated Convolutional Neural Network model, laying the groundwork for the final system. Although the model achieved a low performance, it provided valuable insights into the challenges of personal color analysis using computer vision. In the upcoming module, efforts will be focused on refining the model, improving its accuracy, and integrating it seamlessly with the existing web application to create a fully functional MVP for the final project.

## IV. References
1. BROWN, J.; ROJAS, A. Determining Personal Colors Guide C-315. [s.l: s.n.]. Available at: <https://pubs.nmsu.edu/_c/C315.pdf >. 
2. XU, Pingyuan et al. Applications of artificial intelligence and machine learning in image processing. Frontiers in Materials, v. 11, p. 1431179, 2024.
3. Simonyan, K., & Zisserman, A. (2015). *Very deep convolutional networks for large-scale image recognition.* In *International Conference on Learning Representations (ICLR)*. arXiv:1409.1556.
4. He, K., Zhang, X., Ren, S., & Sun, J. (2016). *Deep residual learning for image recognition. In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR)* (pp. 770–778).
5. Tan, M., & Le, Q. V. (2019). *EfficientNet: Rethinking model scaling for convolutional neural networks. In Proceedings of the 36th International Conference on Machine Learning (ICML)*, PMLR 97:6105–6114. arXiv:1905.11946.
6. WANG, Shuihua; ZHANG, Yudong. Grad-CAM: understanding AI models. **Comput. Mater. Contin**, v. 76, n. 2, p. 1321-1324, 2023.
7. ARUN, Nishanth et al. Assessing the trustworthiness of saliency maps for localizing abnormalities in medical imaging. **Radiology: Artificial Intelligence**, v. 3, n. 6, p. e200267, 2021.
8. VALOIS, Pedro HV; NIINUMA, Koichiro; FUKUI, Kazuhiro. Occlusion sensitivity analysis with augmentation subspace perturbation in deep feature space. In: **Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision.** 2024. p. 4829-4838.
