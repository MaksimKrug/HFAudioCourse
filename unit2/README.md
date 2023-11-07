## Hands-on exercise

This exercise is not graded and is intended to help you become familiar with the tools and libraries that you will be using throughout the rest of the course. If you are already experienced in using Google Colab, 🤗 Datasets, librosa and 🤗 Transformers, you may choose to skip this exercise.

1. Create a Google Colab notebook.
2. Use 🤗 Datasets to load the train split of the facebook/voxpopuli dataset in language of your choice in streaming mode.
3. Get the third example from the train part of the dataset and explore it. Given the features that this example has, what kinds of audio tasks can you use this dataset for?
4. Plot this example’s waveform and spectrogram.
5. Go to 🤗 Hub, explore pretrained models and find one that can be used for automatic speech recognition for the language that you have picked earlier. Instantiate a corresponding pipeline with the model you found, and transcribe the example.
6. Compare the transcription that you get from the pipeline to the transcription provided in the example.

If you struggle with this exercise, feel free to take a peek at an example solution. Discovered something interesting? Found a cool model? Got a beautiful spectrogram? Feel free to share your work and discoveries on Twitter!

In the next chapters you’ll learn more about various audio transformer architectures and will train your own model!