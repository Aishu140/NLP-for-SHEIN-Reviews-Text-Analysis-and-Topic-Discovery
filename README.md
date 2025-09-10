# NLP-for-SHEIN-Reviews-Text-Analysis-and-Topic-Discovery
The goal of this project is to analyze customer reviews from SHEIN, a global e-commerce fashion platform, using Natural Language Processing (NLP) techniques. The project aims to:
Preprocess raw text reviews to remove noise and irrelevant content.
Identify key words and topics that frequently appear in customer feedback.
Discover latent patterns and topics using LDA (Latent Dirichlet Allocation).
Explore semantic relationships between words using Word2Vec embeddings.

Dataset : 
The dataset consists of 15 sample SHEIN customer reviews covering aspects such as product quality, sizing, delivery, customer service, and overall shopping experience.
Each review contains text, rating, and sentiment (positive, neutral, negative).
Example reviews:
“Love the dress! Perfect fit and excellent quality.”
“The delivery was late, but the product is good.”
“Fabric quality is poor, not worth the price.”

Methodology
1. Text Preprocessing
Convert all text to lowercase for uniformity.
Remove punctuation and special characters.
Tokenize text into words using NLTK.
Remove stopwords (common words like “the,” “and,” etc.) to focus on meaningful words.

2. TF-IDF Analysis
TF-IDF (Term Frequency–Inverse Document Frequency) was applied to extract the top keywords in each review.
This helps identify which words are most important across the reviews, e.g., "delivery," "quality," "dress," "service."

3. Word2Vec Embeddings
Trained a Word2Vec model on the preprocessed reviews to capture semantic relationships between words.
Word2Vec represents words in a high-dimensional vector space, where similar words are close to each other.
Example insights from Word2Vec:
Words like "dress" and "clothes" are semantically similar.
"Delivery" is related to "shipping" and "packaging".
Visualized embeddings using PCA, which reduces the vector space to 2 dimensions for plotting.

4. Topic Modeling with LDA
Applied Latent Dirichlet Allocation (LDA) to discover 3 main topics in the reviews.
Example topics identified:
Topic 1: Product Quality & Material – (“quality,” “fabric,” “stitching”)
Topic 2: Delivery & Packaging – (“delivery,” “shipping,” “packaged”)
Topic 3: Customer Service & Sizing – (“service,” “size,” “return”)
Each review was assigned the most relevant topic based on its content.

Output and Insights
Word2Vec Example Output
Similar words to “dress”: ['clothes', 'top', 'skirt', 'shirt', 'outfit']
Similar words to “quality”: ['fabric', 'material', 'stitching', 'durability', 'fit']
Top Keywords from TF-IDF
"delivery," "quality," "dress," "service," "size" were the most frequent significant words across the reviews.
