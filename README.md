# Next Word Prediction Using LSTM

This project demonstrates a Next Word Prediction model built using LSTM (Long Short-Term Memory) architecture. The model is trained on the text of Shakespeare's "Hamlet" and is designed to predict the next word in a given sequence of words.

## Project Overview

This project implements the following steps:
1. **Data Collection**: Shakespeare's "Hamlet" text is loaded using NLTK’s Gutenberg corpus.
2. **Data Preprocessing**: The text is processed to create word indices, tokenized sequences, and padded inputs.
3. **Model Building**: A sequential LSTM model is built using Keras.
4. **Training and Evaluation**: The model is trained on tokenized sequences and evaluated on test data.
5. **Prediction**: A function is provided to predict the next word given an input sequence.
6. **Saving the Model**: The trained model and tokenizer are saved for future use.

## Directory Structure

- `LSTM.ipynb`: Jupyter notebook containing the full code and explanation of each step in the project.
- `app.py`: Streamlit app to interact with the model for next word prediction.
- `next_word_lstm.h5`: Saved model file.
- `tokenizer.pickle`: Saved tokenizer file.
- `requirements.txt`: List of required packages.

## Setup and Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/Next-Word-Prediction-LSTM.git
    cd Next-Word-Prediction-LSTM
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Jupyter Notebook**:
    - Open `LSTM.ipynb` in Jupyter Notebook or Jupyter Lab and execute the cells step-by-step.

4. **Run the Streamlit App**:
    - To interact with the model, run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

## Usage

- **Train the Model**: Run `LSTM.ipynb` to train the model and save it along with the tokenizer.
- **Next Word Prediction**: The Streamlit app takes a sequence of words as input and predicts the next word.

## Model Architecture

The LSTM model consists of:
- An embedding layer for word representation.
- Two stacked LSTM layers with dropout regularization.
- A dense output layer with softmax activation for next word prediction.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
