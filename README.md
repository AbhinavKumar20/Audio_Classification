Urban Sound Classification using Convolutional Neural Networks (CNN)
Overview
This project focuses on classifying urban sounds into ten distinct categories using Convolutional Neural Networks (CNN). The dataset comprises ten classes: air_conditioner, car_horn, children_playing, dog_bark, drilling, engine_idling, gun_shot, jackhammer, siren, and street_music. The primary goal of the project was to develop a reliable classification model to accurately identify these urban sound categories.

**Dataset**
The Urban Sound dataset used in this project consists of audio clips from various urban environments. Each class contains a collection of sound samples, with a total of 8732 clips. The dataset is split into training and testing sets, with appropriate class distribution to ensure representative samples for each category.

**Methodology**
* Data Preprocessing
Several techniques were employed to preprocess the audio data before feeding it into the CNN model:

Mel-frequency cepstral coefficients (MFCC): MFCCs were extracted from the audio clips to represent the spectral characteristics of the sound.
Waveform Plots: Visual representations of audio waveforms were generated to provide a basic understanding of each sound class.
Spectrogram: Spectrograms were computed to capture the time-frequency representation of the audio signals.

**Model Architecture**
A Convolutional Neural Network (CNN) architecture was chosen due to its effectiveness in handling image-like data. The model architecture consisted of convolutional layers for feature extraction, followed by fully connected layers for classification. The model was trained using the extracted MFCC features and the corresponding one-hot encoded labels.

**Training and Evaluation**
The dataset was randomly split into training and testing sets. The model was trained on the training data with an appropriate optimization algorithm (e.g., Adam optimizer) and a suitable loss function (e.g., categorical cross-entropy). The training process was monitored using accuracy and loss metrics. After training, the model was evaluated on the test set to assess its performance on unseen data.

**Results**
The CNN model achieved an impressive test accuracy of 80%. This suggests that the model is effective in distinguishing between the different urban sound categories. The spectrograms, MFCCs, and waveform plots created during preprocessing provided valuable insights into the audio data and likely contributed to the model's success.

**Conclusion**
This project demonstrates the feasibility of using Convolutional Neural Networks for urban sound classification. With a test accuracy of 80%, the model effectively categorizes urban sounds into ten distinct classes. The combination of MFCCs, spectrograms, waveform plots, and one-hot encoding helped achieve this level of accuracy. Further enhancements could involve experimenting with different model architectures, incorporating data augmentation techniques, or exploring transfer learning for improved performance.

