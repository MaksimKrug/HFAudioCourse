## Hands-on exercise

It’s time to get your hands on some Audio models and apply what you have learned so far. This exercise is one of the four hands-on exercises required to qualify for a course completion certificate.

Here are the instructions. In this unit, we demonstrated how to fine-tune a Hubert model on marsyas/gtzan dataset for music classification. Our example achieved 83% accuracy. Your task is to improve upon this accuracy metric.

Feel free to choose any model on the 🤗 Hub that you think is suitable for audio classification, and use the exact same dataset marsyas/gtzan to build your own classifier.

Your goal is to achieve 87% accuracy on this dataset with your classifier. You can choose the exact same model, and play with the training hyperparameters, or pick an entirely different model - it’s up to you!

For your result to count towards your certificate, don’t forget to push your model to Hub as was shown in this unit with the following **kwargs at the end of the training:

```
kwargs = {
    "dataset_tags": "marsyas/gtzan",
    "dataset": "GTZAN",
    "model_name": f"{model_name}-finetuned-gtzan",
    "finetuned_from": model_id,
    "tasks": "audio-classification",
}
trainer.push_to_hub(**kwargs)
```