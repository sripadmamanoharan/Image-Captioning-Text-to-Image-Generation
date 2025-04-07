# Image Captioning & Text-to-Image Generation  
**Computer Vision + NLP Project | Team 10**  
**By:** Sri Padmavathi Manoharan, Sashank Reddy Talakola, Sai Jahnavi Damacharla  

---

## Project Overview

This project explores two major AI tasks:
1. **Image Captioning:** Generating descriptive text from images using deep learning models.
2. **Text-to-Image Generation:** Creating high-quality images from textual prompts using Stable Diffusion and CLIP.

Both tasks were implemented using the **Flickr30k** dataset, which contains over 31,000 images with multiple human-annotated captions.

---

##  Objectives

- Build a robust image captioning model using **ResNet-34 + Transformer decoder**.
- Generate realistic images from text using **Stable Diffusion** guided by **CLIP embeddings**.
- Evaluate both systems using metrics like **BLEU**, **FID**, and **CLIP Similarity Score**.

---

##  Image Captioning

### 🔨 Methodology
- **Feature Extraction:** ResNet-34, EfficientNet, ViT, Swin Transformer
- **Captioning Models:** LSTM, GRU, Transformer decoder
- **Attention Mechanism:** Used to focus on key image regions
- **Evaluation:** BLEU Score (Best: **0.309**)

###  Example Output
**Input:** 🐶 A dog jumping over a hurdle  
**Generated Caption:** "A brown dog jumps over a hurdle"

---

##  Text-to-Image Generation

### ⚙️ Methodology
- **Architecture:** CLIP (text encoding) + Stable Diffusion (image synthesis)
- **Training:** Fine-tuned using Flickr30k captions and images
- **Evaluation Metrics:**  
  - Inception Score (IS)  
  - Frechet Inception Distance (FID)  
  - CLIP Similarity Score

### Sample Prompts
- "A man in a red shirt standing on a grassy hill" → 🧍‍♂️🌿  
- "A group of people playing soccer in a park" → ⚽🏃‍♀️🏃‍♂️

---

##  Results Summary

| Task                   | Best Model/Method       | Score     |
|------------------------|-------------------------|-----------|
| Image Captioning       | ResNet-34 + Transformer | BLEU: 0.309 |
| Text-to-Image Gen.     | CLIP + Stable Diffusion | Strong CLIP Similarity |

---

##  Key Learnings

- **Transformer decoders** outperform LSTMs and GRUs in long-sequence captioning.
- **Vocabulary tuning** and **sequence length optimization** significantly impact performance.
- **CLIP + Diffusion** models generate semantically rich images from text with great diversity.

---

## Tools & Technologies

- Python  
- PyTorch  
- HuggingFace Transformers  
- Stable Diffusion  
- CLIP (OpenAI)  
- Flickr30k Dataset  
- BLEU / FID / CLIP Similarity

---

## Team Contributions

- **Sri Padmavathi Manoharan** – Image captioning (Transformer), attention mechanism, BLEU evaluation  
- **Sashank Reddy Talakola** – Feature extraction models, Stable Diffusion implementation  
- **Sai Jahnavi Damacharla** – Text preprocessing, CLIP embeddings, evaluation metrics  

