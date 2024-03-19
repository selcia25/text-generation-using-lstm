# Text Generation using LSTM

This project explores text generation using LSTM (Long Short-Term Memory) neural networks. It trains an LSTM model on a dataset of Medium article titles to predict the next word in a sequence, allowing for the generation of new text based on a seed text.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/selcia25/text-generation-using-lstm.git
   ```

2. Install the required libraries:
   ```sh
   pip install pandas numpy tensorflow matplotlib
   ```

## Dataset

The dataset used for training the model is a collection of Medium article titles. The dataset (`medium_data.csv`) contains a single column named `title` with the titles of the articles.

## Model Training

1. Preprocess the data: Clean the text by removing unnecessary characters and tokenize the text using the `Tokenizer` class from Keras.

2. Generate input sequences: Create input sequences of varying lengths to train the model.

3. Pad sequences: Pad the input sequences to ensure uniform length.

4. Build the LSTM model: Construct a Sequential model with an Embedding layer, a Bidirectional LSTM layer, and a Dense output layer with a softmax activation.

5. Compile the model: Compile the model using the Adam optimizer and categorical crossentropy loss function.

6. Train the model: Train the model on the input sequences and corresponding labels.

## Usage

1. Run the script to train the model.

2. Use the trained model to generate text by providing a seed text and specifying the number of words to generate.

## Examples

Here are some examples of generating text using the trained model:

- Seed text: "implementation of"
  - Generated text: "implementation of rnn lstm"

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
