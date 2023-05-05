# Automatic-Speech-Recognition-with-Synthetic-Speech
Introduction to Deep Learning (11.785) - Project 

This paper explores a solution to one of the main factors stunting the acceleration of
state-of-the-art speech recognition systems. This is the acquisition of high-quality
data. To remove excess costs in acquiring the required data, the area of synthetic
speech generation and its applications in training is being tested. This paper
aims to test the hypothesis of solely synthetic speech being capable of training a
speech recognizer that is comparable to a model trained using actual human speech.

# How to setup synthetic speech generation and recognition pipeline
In the VITS synthetic speech generation notebook, add the transcript for which you would like to generate synthetic speech. Once VITS has completed generating the .WAV files, convert them to MFCCs. This is a required step as the LAS architecture is setup to read audio in the form of MFCCs.

To replicate our results, we use the transcripts from Librispeech train-clean-360.

After the audio is converted to MFCCs, use the LAS notebook to start training the speech recognizer. The notebook automatically computes the Word Error Rate and Levenstein Distance in the train function. We encourage users to experiment with generating large amounts of data and train LAS to see how far synthetic speech can take us.

We value any feedback and are open to questions. Please feel free to shoot the authors questions and open issues on Github.
