# Worker Fatigue Detection from Voice

This is my EE769 course project for **Introduction to Machine Learning, IIT Bombay**.  
The project explores whether worker fatigue can be detected using only short voice recordings.

Instead of using expensive sensors like EEG or wearables, I used acoustic speech features and machine learning models to classify fatigue levels from voice. The main idea is to compare a person’s current voice with their own normal/rested voice, instead of comparing across different people.

---

# Problem Statement

Given a short voice recording, predict whether the speaker is:

- `alert`
- `mild_fatigue`
- `fatigued`

The model also gives a continuous fatigue score between 0 and 1.

---

# Motivation

Fatigue is a real issue in industries like transportation, mining, shipping, construction, and manufacturing. Tired workers can make more mistakes, cause accidents, and reduce productivity.

Most existing methods are not ideal for daily use:

- self-reporting is unreliable
- EEG and medical sensors are expensive and invasive
- wearables are not always practical

Voice is a good alternative because it is non-invasive and easy to capture.

---

# Dataset

I used the **RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)** dataset.

Since there is no public fatigue dataset available, I used emotions as a proxy for fatigue levels.

Dataset link:  
https://zenodo.org/records/1188976

After downloading, place the dataset inside:

```plaintext
data/RAVDESS/
