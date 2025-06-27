# Punctuation Restoration Using Transformer Models

Punctuation restoration is the process of adding missing punctuation marks to text, often from speech-to-text outputs. In this research, we focus on improving punctuation restoration in the Bangla language, specifically adding periods, commas, question marks, and exclamation marks.

## Data

#### Bangla

The Bangla datasets can be found in the data/bn directory.

## Model Architecture

We implement a pretrained Transformer-based model (such as BERT) for punctuation restoration. The model includes a Transformer encoder, followed by a bidirectional LSTM and a linear layer to predict punctuation at each position in the text.
![model_architecture](https://github.com/user-attachments/assets/1e9f9f65-94b6-49a8-8578-1d4b501a736d)

## Here Augmentation program commented in train.py

#### Bangla Supported Models

```
bert-base-multilingual-cased
bert-base-multilingual-uncased
xlm-mlm-100-1280
distilbert-base-multilingual-cased
xlm-roberta-base
xlm-roberta-large
```

## Pretrained Model Selection

XLM-RoBERTa-large with Augmentation for Bangla is Available [here](https://drive.google.com/file/d/1X2udyT1XYrmCNvWtFpT_6jrWsQejGCBW/view?usp=sharing)

For Bangla Output Expectations

```text
বিংশ শতাব্দীর বাংলা মননে কাজী নজরুল ইসলামের মর্যাদা ও গুরুত্ব অপরিসীম। একাধারে কবি, সাহিত্যিক, সংগীতজ্ঞ, সাংবাদিক, সম্পাদক, রাজনীতিবিদ এবং সৈনিক হিসেবে অন্যায় ও অবিচারের বিরুদ্ধে নজরুল সর্বদাই ছিলেন সোচ্চার। তার কবিতা ও গানে এই মনোভাবই প্রতিফলিত হয়েছে। অগ্নিবীণা হাতে তার প্রবেশ, ধূমকেতুর মতো তার প্রকাশ! যেমন লেখাতে বিদ্রোহী, তেমনই জীবনে – কাজেই "বিদ্রোহী কবি", তার জন্ম ও মৃত্যুবার্ষিকী বিশেষ মর্যাদার সঙ্গে উভয় বাংলাতে প্রতি বৎসর উদযাপিত হয়ে থাকে। নজরুলের রচনাবলীর মধ্যে বিদ্রোহ, ভালোবাসা, সাম্য এবং মানবতার অমোঘ বার্তা ধ্বনিত হয়েছে। তার প্রতিটি শব্দ যেন একেকটি আগুনের ফুলকি, প্রতিটি কবিতা যেন প্রতিবাদের ভাষা! এমন বিদ্রোহী চেতনার কবি নজরুল বাংলা সাহিত্য ও সঙ্গীতে এক অনন্য প্রতিভা।
```

## Test

Assess Trained Models on Processed Data with the test Module.
