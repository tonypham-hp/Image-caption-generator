# Image Caption Generator

**Deep Learning project** for generating natural-language captions from images using VGG16 + LSTM.

A complete end-to-end pipeline including feature extraction, caption preprocessing, model training, BLEU evaluation, and caption prediction.


# Features
- **Image Feature Extraction** using pretrained **VGG16**  
- **Caption Tokenization** & vocabulary generation  
- **Encoder–Decoder model** with LSTM  
- BLEU-1 & BLEU-2 evaluation  
- Generate captions for any new image  

# Notebook  
**Kaggle Notebook:**  https://www.kaggle.com/code/tonypham04/image-caption-generator/notebook
# Model Architecture
- **Encoder:** VGG16 (without top) → Dense → Dropout  
- **Decoder:** Embedding → LSTM → Dense Softmax  
- **Output:** Word-by-word caption generation  

# Training
- Sequence generation for captions  
- Teacher forcing during training  
- Validation split + loss visualization  
- Model & tokenizer saving (`.h5`, `.pkl`)  

# Evaluation
- BLEU-1: Measures unigram precision.
- BLEU-2: Measures bigram precision.
- Display of actual vs predicted captions.
