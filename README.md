# TEXT SUMMARIZATION TOOL

*Company*: CODTECH IT SOLUTIONS

*NAME*: PASUPULATE HANISHKA ROYAL

*INTERN ID*: CTO6DG22

*DOMAIN*: ARTIFICIAL INTELLIGENCE

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTOSH  

*DESCRIPTION*: The function read_article(file_name) reads a text file and processes the content into sentences. It splits the text based on the period (.) to form individual sentences. Then, it cleans each sentence by removing non-alphabetic characters and tokenizing the words.
The function sentences_similarity(sent1, sent2, stopwords=None) measures how similar two sentences are using the cosine similarity metric. The cosine similarity determines the closeness between two word vectors.
vector1 = [0] * len(all_words)
vector2 = [0] * len(all_words)
A similarity matrix is built using gen_sim_matrix(sentences, stop_words=None). This matrix represents the relationships between all sentences. Each sentence is compared with every other sentence to determine how connected they are.
The script constructs a graph representation of the sentences using the networkx library, and applies the PageRank algorithm to rank sentences based on importance.
The highest-ranked sentences are selected to form the final summary. The generate_summary(file_name, top_n=5) function picks the top sentences and assembles them into a readable format.
ranked_sentence = sorted(((scores[i], s) for i, s in enumerate(sentences)), reverse=True)
summarize_text.append(" ".join(ranked_sentence[i][1]))





