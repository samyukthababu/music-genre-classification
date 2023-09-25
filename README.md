# Music Genre Classification

The notebooks show the code used to perform multi-class classification of images and audio files into 10 classes (music genres) for the dataset taken from Kaggle: [GTZAN Dataset - Music Genre Classification](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification). 

Classification of images was implemented using Feed-Forward Neural Network (FNN) and Convolutional Neural Network (CNN) (3 different architectures) for 50 and 100 epochs. 

The accuracy for the 4 networks for 50 epochs are shown in the table below: 

| Network Architectures | Training Accuracy | Validation Accuracy | Test Accuracy |
| --- | --- | --- | --- |
| FNN + ReLU + Adam | 84.55% | 41.40% | 45.54% |
| CNN + ReLU + Adam | 100% | 45.71% | 46.53% |
| CNN + ReLU + Batch Normalisation + Adam | 100% | 65.03% | 56.41% |
| CNN + ReLU + Batch Normalisation + RMSprop | 33.08% | 30.55% | 31.25% | 

The accuracy for the 4 networks for 100 epochs are shown in the table below: 

| Network Architectures | Training Accuracy | Validation Accuracy | Test Accuracy |
| --- | --- | --- | --- |
| FNN + ReLU + Adam | 96.60% | 40.83% | 47.52% |
| CNN + ReLU + Adam | 100% | 48.02% | 49.50% |
| CNN + ReLU + Batch Normalisation + Adam | 100% | 61.76% | 56.41% |
| CNN + ReLU + Batch Normalisation + RMSprop | 79.11% | 39.06% | 45.94% | 

Classification of audio was implemented using Long-Short Term Memory (LSTM). Data Augmentation was performed using Generative Adversarial Network (GAN), after which classification was performed. These two networks were compared and the accuracy for 50 epochs is shown in the table below:

| Network Architectures | Training Accuracy | Validation Accuracy | Test Accuracy |
| --- | --- | --- | --- |
| LSTM | 51.65% | 48.05% | 52.85% |
| LSTM + Augmented data | 35.58% | 35.30% | 37.61% |
