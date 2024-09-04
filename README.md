
# Article Spinner using Markov Model

## Overview
This project is an implementation of an article spinner using a Markov Model, designed to generate variations of articles or text while maintaining readability. The model uses techniques such as tokenization, detokenization, and probabilistic word prediction to create new content variations.

## Dataset
The dataset used in this project is the **BBC Text Classification Dataset**, which consists of various news articles labeled by category (e.g., business, tech, sports). The dataset is pre-processed using the following steps:
- **Loading the dataset**: The dataset is loaded into a DataFrame for easy manipulation and analysis.
- **Analyzing Label Distribution**: The labels are analyzed to understand the content distribution across different categories.

## Key Functionalities
1. **Text Processing**:
   - Tokenization using `nltk` to break down sentences into individual tokens.
   - Detokenization using `TreebankWordDetokenizer` to reconstruct text from tokens while maintaining proper punctuation and spacing.
   
2. **Markov Model Implementation**:
   - A second-order Markov model is used to generate new text by predicting the middle word based on the two words. This allows for probabilistic generation of text sequences.

3. **Article Spinning**:
   - Creates multiple variations of the given text, enabling content generation that is grammatically correct but may vary in logical coherence.
   - Utilizes techniques like random selection (`np.random.choice`) for generating text samples.

## Installation and Usage
To use the notebook:
1. Clone the repository:
   ```bash
   git clone https://github.com/
   cd Article-Spinner-using-Markov-Model
   ```
2. Install the required dependencies:
   ```bash
   pip install pandas numpy nltk
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Article_Spinner_using_Markov_Model.ipynb
   ```

## Future Enhancements
- Incorporate more sophisticated NLP models to improve logical coherence.
- Add support for other languages and datasets.
- Implement a web-based interface for ease of use.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Dataset sourced from [BBC News Classification Dataset](https://lazyprogrammer.me/course_files/nlp/bbc_text_cls.csv).
- Inspired by various NLP resources and tools.
