# Movie Recommendation System using Softmax Deep Neural Network

<p align="justify">
A Softmax Deep Neural Network (DNN) is a type of neural network that uses the softmax function in its output layer to classify inputs into multiple categories. The softmax function converts the output logits (raw prediction values) into probabilities that sum to 1, making it ideal for multi-class classification tasks. In this network, multiple hidden layers (hence "deep") are used to learn complex patterns from data, while the softmax layer helps in selecting the most likely class or category.
</p>

## 1. Loading and Merging Datasets
- Load the movie dataset, containing user ratings, movie titles, and other relevant information.
- Merge any required datasets (e.g., user data, movie metadata) to create a unified dataset.

## 2. Creating a Refined Dataset
- Create a final refined dataset with unique `user ID`, `movie title`, and `ratings`.
- Ensure the dataset contains no duplicates and is structured properly for processing.

## 3. Encoding Users and Movie Titles
- Encode `user IDs` and `movie titles` using label encoders or other encoding techniques.
- Ensure no missing values remain after encoding to work seamlessly with Deep Neural Networks (DNNs).

## 4. Splitting Data into Training and Testing Sets
- Split the dataset into training and testing subsets.

## 5. Defining Number of Factors for the Embedding Layer
- Decide on the number of latent factors (embedding dimensions) for both `user IDs` and `movie titles` to be used in the embedding layer.

## 6. Normalizing the Labels
- Normalize the ratings to a suitable range (e.g., [0, 1]) to improve model performance.

## 7. Building the Deep Neural Network
- Construct a neural network model with:
  - Embedding layers for users and movies.
  - Dense layers to learn from embeddings.
  - A **Softmax** output layer to predict rating probabilities.

## 8. Getting Movie Recommendations for a Given User
- Define a function that takes a `user ID` as input and outputs recommended movies based on the trained model.

## 9. Summing up the Code into a Recommender System Function
- Wrap the entire process into a single function:
  - Train the model using the training dataset.
  - Validate the model on the test dataset.
  - Generate movie recommendations for users based on their past interactions.

