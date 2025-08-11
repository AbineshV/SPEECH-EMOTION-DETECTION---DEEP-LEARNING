# Speech Emotion Recognition Using Multi-Channel Audio Spectrograms and Image-Based Deep Learning

📌 Overview

   This project presents a Speech Emotion Recognition (SER) system that converts audio signals into multi-channel visual representations (spectrograms, MFCCs, and composite     acoustic features) and applies a modified Xception deep learning architecture for emotion classification.
   It achieves 77.03% accuracy on the RAVDESS dataset using speaker-independent evaluation (Leave-One-Speaker-Out cross-validation).

🎯 Key Features

   Multi-channel input:

   Channel 1: Spectrogram

   Channel 2: MFCCs

   Channel 3: Composite features (Zero Crossing Rate, RMS Energy, Chroma)

   Modified Xception architecture: Retains entry & middle flows; removes exit flow for better speech feature extraction.
 
   Generalized Mean (GeM) pooling: Learns optimal pooling strategy to preserve discriminative features.

   Data augmentation: Noise addition, time stretching, time shifting, and pitch shifting for robust generalization.

   Evaluation strategy: Leave-One-Speaker-Out (LOSO) cross-validation for true speaker independence.

🛠 Tech Stack

   Language: Python

   Frameworks: TensorFlow / Keras

   Libraries: NumPy, Librosa, Matplotlib, Scikit-learn

   Dataset: RAVDESS

📊 Results

   Model	Classifier	Accuracy

   Xception	MLP	77.03%

   Xception	SVM	66.76%

   AlexNet	MLP	72.88%

   AlexNet	SVM	56.08%

   Xception + MLP achieved the best performance.

   Multi-channel input & GeM pooling significantly improved classification of similar emotions.

📌 Future Work

   Integration with real-time SER for voice assistants.

   Explore attention mechanisms for improved feature focus.

   Expand to multilingual emotion recognition.

👨‍💻 Authors

   V Abinesh

   R T Surya

   G V Hariharan

   (School of Electronics Engineering, VIT Chennai)
