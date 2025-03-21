# Logo Similarity
This project aims to group company logos based on visual similarity. For each company, there are multiple images of its logo, and the goal is to identify and group these images according to the company they belong to. The program analyzes and organizes the logos, correctly associating each set of images with the corresponding company.

## Stages
### Stage I: Image Collection via Web Scraping
In the first stage, using the dataset `logos.snappy.parquet`, which contains the domains of multiple websites, a web scraper was implemented to collect as many images from these sites as possible. The primary goal was to identify images that could correspond to logos.

### Stage II: Feature Extraction Methods
In the second stage, the images from the dataset are loaded. Two methods are used for feature extraction: applying Principal Component Analysis (PCA) and using the deep learning model ResNet50.

### Stage III: Analysis of Unsupervised Clustering Results
In the final stage, based on the extracted features, an unsupervised clustering method was applied to group the logos based on visual similarity. The connections between the classified logos and their domains from the dataset were established. Various metrics were then used to evaluate how well the clustering correctly assigned logos belonging to the same companies. Depending on the method used, different results were obtained and compared.

For a complete view of the code and results obtained, please access [logo_similarity.ipynb](logo_similarity.ipynb).
