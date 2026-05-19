# Influencer Profiling System Using Machine Learning and Deep Learning Techniques

This project presents a multimodal influencer profiling system that automatically classifies social media influencers using both textual and visual content from Instagram posts. The framework combines Machine Learning and Deep Learning techniques to improve influencer categorization and assist brands in identifying suitable influencers for targeted marketing campaigns.

## Objectives

* Develop an automated influencer classification framework
* Analyze both textual captions and visual content from influencer posts
* Compare Machine Learning and Deep Learning approaches
* Improve influencer categorization using multimodal learning

## Technologies & Models Used

### Text Processing

* BERT (BERT-base-multilingual-cased)
* Text Embeddings (768-Dimensional)

### Image Processing

* InceptionV3
* Image Embeddings (1024-Dimensional)

### Machine Learning Models

* Random Forest
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)
* Gaussian Naive Bayes

### Deep Learning

* Attention-Based Neural Network
* Multimodal Fusion Architecture

## Dataset

The project uses a large-scale Instagram influencer dataset containing:

* 33,000+ influencers
* 1.6 million posts
* Captions, hashtags, images, engagement metrics, and influencer profile information

For efficient training and balanced category representation:

* 1,500 influencers were selected
* 20 posts per influencer were sampled

## Data Preprocessing

### Text Preprocessing

* URL and hyperlink removal
* Emoji-to-text conversion
* Tokenization using BERT tokenizer
* Cleaning special characters and extra spaces

### Image Preprocessing

* Image resizing to 299×299
* Pixel normalization
* Removal of corrupted images

## Model Architecture

The framework consists of:

1. **BERT Text Encoder** for extracting semantic caption embeddings
2. **InceptionV3 Image Encoder** for extracting visual embeddings
3. **Multimodal Fusion Layer** combining text and image embeddings
4. **Attention Mechanism** to identify the most representative influencer posts
5. **Neural Classification Head** for final influencer category prediction

## Results

| Model                | Text   | Image  | Text + Image |
| -------------------- | ------ | ------ | ------------ |
| Random Forest        | 45%    | 73.33% | 75%          |
| KNN                  | 39%    | 58%    | 74%          |
| SVM                  | 51%    | 78%    | 83%          |
| Gaussian Naive Bayes | 27.67% | 65%    | 76.33%       |
| Neural Classifier    | 56%    | 79%    | 85%          |

### Key Findings

* Image features performed better than text features
* Multimodal fusion significantly improved classification accuracy
* Attention-based neural networks achieved the best performance
* The final neural classifier achieved **85% accuracy**

## Business Impact

This system can help:

* Brands identify suitable influencers
* Automate influencer categorization
* Improve marketing campaign targeting
* Reduce manual influencer selection effort

## Future Scope

* Integration with CLIP or ViLT models
* Real-time influencer recommendation systems
* Inclusion of engagement metrics like likes/comments
* Video and audio-based influencer profiling
* Explainable AI for influencer recommendation systems

## Disclaimer

This project is developed for academic and research purposes only. The original dataset and influencer content belong to their respective owners.
