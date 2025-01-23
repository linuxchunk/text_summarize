# Text Summarizer

A Streamlit-based web application that generates extractive summaries from text documents using Natural Language Processing (NLP) techniques and the PageRank algorithm.

## Features

- Upload and process text documents
- Automatic text summarization
- Interactive web interface
- Extractive summarization using sentence similarity and PageRank
- Configurable summary length

## Installation

1. Clone this repository:
```bash
git clone https://github.com/linuxchunk/text_summarize.git
cd text-summarizer
```

2. Install the required dependencies:
```bash
python -m venv env
source env/bin/activate
pip install -r requirements.txt
```

## Usage

1. Run the Streamlit application:
```bash
streamlit run main.py
```

2. Open your web browser and navigate to the URL shown in the terminal (typically `http://localhost:8501`)

3. Upload a text file using the file uploader

4. The application will automatically generate a summary of the text

## How It Works

The text summarization process follows these steps:

1. **Text Processing**: The input text is split into sentences and preprocessed to remove special characters
2. **Sentence Similarity**: Calculates similarity between sentences using cosine distance
3. **Graph Building**: Creates a similarity matrix and converts it to a graph
4. **Ranking**: Uses PageRank algorithm to rank sentences by importance
5. **Summary Generation**: Extracts the top-ranked sentences to create the final summary

## Dependencies

- streamlit: Web application framework
- nltk: Natural Language Processing toolkit
- numpy: Numerical computing library
- networkx: Graph operations library
- scipy: Scientific computing library

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- Built using Streamlit framework
- Uses NLTK for natural language processing
- Implements PageRank algorithm for sentence ranking

