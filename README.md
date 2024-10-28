# CNN_based_image_classification
# Aim:
The objective was to develop and train a Convolutional Neural Network(CNN) to classify images from the CIFAR-10 dataset into 10 categories and evaluate its performance using precision, recall, F1-score, and accuracy metrics.
# Dataset:
- CIFAR-10 Dataset - A dataset consist of 60,000 images categorized into 10 different classes, such as airplanes,automobiles, birds, cats, dogs, etc.
- Dataset Split -
- Training Set: 70%
- Validation Set: 15%
- Test Set: 15%
# Data Preprocessing:
- Applied data augmentation techniques to resized the images and normalized the pixel values to be between 0 and 1.
- Data augmentation increases the diversity of the training set by modifying the images which helps in preventing overfitting.
# CNN Architecture layers used:
- Convolution layer as it will extract spatial features and it is basically suitable for large image datasets.
- MaxPooling layers for reducing high dimensions.
- Dropout Layer to prevent overfitting by randomly setting a fraction of inputs to zero during training.
- Fully Connected Layers (dense layers) to get final output.
# Model Training:
- Trained the model using the Adam optimizer and sparse categorical crossentropy loss.
- Epochs used 50 and bath size provided 64.
- Manually tune the hyperparameters as it is difficult to use GridSearch or any other technique with limited computational resource and by checking performance metrics on the validation set.
# Model Evaluation:
1) Confusion Matrix Analysis:
- Certain classes may be misclassified more often due to visual similarities.
2) Overall Performance:
- The model achieves around 79% accuracy but struggles with certain classes due to overlapping features.
# Class-wise Performance :
1) Strong Performers
- Class 8 : Exhibited the highest precision (0.88) and recall(0.87), indicating robust performance in distinguishing this class.
- Class 1 : Achieved high recall (0.92) suggesting clear visual distinction in this category.
2) Classes with Misclassifications
- Class 3 : Showed lower recall (0.61) and F1-score (0.64), indicating difficulties in correctly identifying these images.
# Further Recommendations:
- Adding more convolutional layers or applying transfer learning techniques could enable the model to learn more complex features and improve the overall performance.
- Hyperparameter Tuning can be done by experimenting with different filters, optimizers, epochs for better performance.
- Addressing Class Imbalances using techniques like class weighting or SMOTE or undersampling to ensure all classes are equally represented during training.
