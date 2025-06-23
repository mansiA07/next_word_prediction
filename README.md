🧠 Next Word Prediction with LSTM
This project is a simple web-based application built using Streamlit that predicts the next word in a sequence using a trained LSTM model on Shakespeare's Hamlet.

📌 Project Overview
The application:

Takes a text input from the user.

Uses a pre-trained LSTM model to predict the next most likely word.

Displays the predicted word to the user in real-time via a web interface.

🗂️ Project Structure
bash
Copy
Edit
.
├── app.py                  # Streamlit app script
├── hamlet.txt             # Corpus used for training
├── next_word_lstm.h5      # Trained LSTM model
├── tokenizer.pickle       # Tokenizer used during training
└── README.md              # Project documentation (this file)
🧪 Model Details
Model Type: LSTM (Long Short-Term Memory)

Framework: TensorFlow/Keras

Training Dataset: hamlet.txt (William Shakespeare's Hamlet)

Input: A sequence of words (e.g., "To be or not to be")

Output: The most probable next word based on training data

🚀 How to Run the App
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/mansiA07/next_word_prediction
cd next_word_prediction
2. Install Requirements
bash
Copy
Edit
pip install -r requirements.txt
If requirements.txt is missing, use:

bash
Copy
Edit
pip install streamlit tensorflow numpy
3. Run the App
bash
Copy
Edit
streamlit run app.py
🖼️ Demo
Enter a phrase like "To be or not to be".

Click Predict Next Word.

The app will predict and display the next most likely word from the Hamlet corpus.

📦 Dependencies
tensorflow

numpy

streamlit

pickle

📝 Notes
The model and tokenizer are trained using only the hamlet.txt file. For production usage, consider training on larger and more diverse corpora.

Only the final word of the sequence is predicted.

Prediction quality may vary due to limited training data and corpus style.

📚 Future Improvements
Add the ability to generate multiple next words.

Fine-tune or retrain the model with larger datasets.

Add part-of-speech tagging or grammar-aware modeling.

Extend to sentence generation or story completion.

👩‍💻 Author
Mansi Arora

