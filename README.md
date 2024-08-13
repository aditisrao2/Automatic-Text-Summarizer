# Automatic Text Summarizer

Developed an Automatic Text Summarizer using NLP libraries like SpaCy, NLTK and Sumy.

## About
Automatic summarization is a renowned approach which is used to reduce a document to its main ideas.

It refers to the technique of condensing a lengthy text document into a succinct and well-written summary that captures the essential information and main ideas of the original text, achieved by highlighting the significant points of the document.

The goal of automatic text summarization is presenting the source text into a shorter version with semantics.

## Data Collection
Users are provided with three options for providing input data :

Users can manually type the text and then request a summary.

Users can open a file containing the text they wish to summarize.

Users can provide a URL link to the specific webpage they want to summarize.

## Summarization Techniques
### 1. SpaCy

In SpaCy summarization, the text is first tokenized and stopwords and punctuation are removed.

Word frequencies are calculated and normalized, then sentences are scored based on these frequencies.

Sentences over 30 words are filtered out, and the top sentences are chosen for the final summary.

### 2. NLTK

This summarization method involves tokenizing the input text into words and sentences, then converting words to lowercase.

Stopwords are removed to focus on significant words. Word frequencies are calculated and normalized for document length.

Sentences are evaluated based on important word frequencies, with a limit of 30 words per sentence for conciseness.

Sentences are ranked by cumulative word frequencies and the top-ranked ones are selected to form the summary, prioritizing key information extraction.

### 3. Sumy

This method uses the LexRank algorithm from the Sumy library in Python for text summarization.

The input text is parsed and tokenized into words and sentences.

LexRankSummarizer ranks sentences based on lexical similarity, considering word overlap and context.

Top-ranking sentences are selected and concatenated to form the final summary.
