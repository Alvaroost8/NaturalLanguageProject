# Medical Text Negation and Uncertainty Detection
This project aims to detect negations, uncertainties, and their scopes in medical texts written in Spanish and Catalan. The work was conducted by four students Joan Bayona, Alejandra Reinares, Álvaro Sáenz-Torre, and Luis Domene under the supervision of Pau Torras and Lei Kang. This project is an assignment part of the "Fundamentals of NLP" course in the Artificial Intelligence program at the Autonomous University of Barcelona (UAB).

## Implemented Methods
### Rule-Based Method
The rule-based method uses handcrafted rules inspired by the NegEx algorithm. The implementation involves:
* Creating lists of negation and uncertainty cues.
* Applying regular expressions to identify the cues and their scopes.

### Machine Learning Method
The machine learning method utilizes Conditional Random Fields (CRF) for sequence tagging. The features used include:
* Part-of-speech tags
* Capitalization information
* Contextual word information (bigrams and trigrams)
* Special indicators for common negation structures in Spanish and Catalan

### Deep Learning Method
The deep learning method employs a bidirectional Long Short-Term Memory (LSTM) network. The features used include:
* Character embeddings
* Word embeddings
* Part-of-speech tags
* Casing information

### Simplified NegEx Adaptation
As a baseline, we also implemented a simplified version of the NegEx algorithm, adapted for Spanish and Catalan. This method involves:

* Searching for negation and uncertainty cues in sentences.
* Determining the scope based on the proximity of medical terms.

### Data Preprocessing
Data preprocessing steps include:
* Removing patient personal information.
* Correcting misspelled words and lemmatization.
* Tokenizing sentences while preserving original text coordinates.

