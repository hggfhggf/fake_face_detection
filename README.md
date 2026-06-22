# AI Fake Face Detection

Solution for an AI-generated face detection task from the **AIIS Winter Contest**.

Training data contains only real faces.  
Test data contains both real and fake faces.  
No external data was used.

## Approach

1. Detected likely fake test images using color-channel statistics.
2. Used those pseudo-labels to train a simple classifier.
3. Generated synthetic fake faces by merging pairs of real images.
4. Extracted **ResNet18** embeddings.
5. Trained **Logistic Regression** on real and synthetic fake samples.

## Result

Best score: **0.92 F1**

## Files

- `data/train` — real face images
- `data/test` — test images
- Notebook solution in Python

## Problem

https://judge.nitro-ai.org/competitions/aiis/aiis-winter-contest/2

## Credits

Problem by **Morariu Tudor** and **Alexandru Ionut Tone**.
