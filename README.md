# Paraphrase-Identification
# Paraphrase Identification with LSTM

## Project Overview
This NLP project develops a paraphrase identification system using a deep bidirectional LSTM (Long Short-Term Memory) network. The goal is to identify semantic similarities between pairs of sentences and determine if they are paraphrases of each other. This involves intricate handling of syntactic and semantic nuances within the text.

## Dataset
The project utilizes the Microsoft Research Paraphrase Corpus, which is known for its varying degrees of paraphrasing across text pairs. This dataset provides a robust foundation for training and evaluating the performance of the LSTM models.

## Technical Approach
### Data Preprocessing
- Tokenization of sentences with special tokens for sentence start, end, and unknown words.
- Vocabulary building from the training dataset to map words to indices.
- Padding sequences to normalize sentence length across the dataset.

### Model Architecture
- **Embedding Layer:** Maps words to a dense vector space.
- **Bidirectional LSTM Layers:** Captures forward and backward dependencies in text.
- **Dense Layer:** A fully connected layer that interprets the LSTM output.
- **Output Layer:** Sigmoid activation to output a probability of the sentence pair being a paraphrase.

### Training
- The model is trained using the Adam optimizer with a binary cross-entropy loss function.
- Validation is performed using a held-out dataset to monitor overfitting and adjust hyperparameters accordingly.

## Results
- Model accuracy and loss are plotted to illustrate learning progress.
- A confusion matrix is generated to visualize the model's performance in classifying paraphrases.
- ROC curves are plotted to evaluate the effectiveness of the model across different threshold settings.

## Usage
To run the analysis and view the performance of the paraphrase identification model:
1. Clone the repository:
