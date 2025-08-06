# Pneumonia Detection: Viral vs Bacterial

A deep learning project to classify chest X-ray images as **Normal**, **Bacterial Pneumonia**, or **Viral Pneumonia**, with visual model explanations and feedback integration.


## 🚀 Features

- **Pneumonia Classification**: Detects whether a chest X-ray shows signs of bacterial pneumonia, viral pneumonia, or is normal.
- **Explainability (Grad-CAM)**: Generates heatmaps to highlight areas in the X-ray that influenced the model's decision.
- **Feedback System**: Doctors can verify predictions and provide the correct label. Images are saved for future retraining.
- **Gradio UI**: Easy-to-use graphical interface for uploading images and viewing predictions + heatmaps.


## 🫁 What is Pneumonia?

Pneumonia is a lung infection that inflames the alveoli and leads to symptoms such as:

* Cough (dry or productive)
* Fever
* Chest pain
* Breathing difficulty

It may result from **bacterial**, **viral**, or less commonly **fungal** infections, medications, or immune conditions. High-risk individuals include those with:

* COPD, Asthma
* Diabetes or heart failure
* Stroke with impaired cough reflex
* Weakened immune systems

Diagnosis involves:

* Physical examination
* Chest X-ray imaging
* Blood tests / sputum culture

![Pneumonia Image](https://img.lb.wbmdstatic.com/vim/live/webmd/consumer_assets/site_images/article_thumbnails/BigBead/pneumonia_everything_you_should_know_bigbead/1800x1200_pneumonia_everything_you_should_know_new_bigbead.jpg)


## 📁 Datasets Used

1. [Chest X-Ray Pneumonia - Paul Timothy Mooney (Kaggle)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)
2. [Pneumonia Dataset - nkifor (Kaggle)](https://www.kaggle.com/datasets/nkifor/pneumonia-dataset)

To ensure dataset integrity:

* **Hashing** was applied to identify and skip duplicate images between datasets. This reduced data leakage and redundancy.


## 📌 Notes

* Trained model weights are **not** included in this repository due to size limitations.
* Grad-CAM is computed using final convolutional layers and overlaid on input images for visual interpretation.
