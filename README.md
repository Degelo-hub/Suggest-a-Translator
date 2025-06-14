# Suggest-a-Translator
Suggest-a-Translator is an intelligent pipeline that analyzes input texts and recommends the most appropriate translator based on semantic content and domain-specific terminology.

What it does:
Domain Classification:
Detects relevant subject areas in the input text based on predefined multilingual terminology lists.

Text Chunking:
Splits the text into manageable chunks (512 tokens) for embedding.

Embedding Generation:
Converts each chunk into high-dimensional embeddings (1024-dim) using a pretrained language model.

Similarity Matching:
Compares the generated embeddings against a database of translator profiles to identify the best semantic match.

Translator Suggestion:
Recommends the most suitable translator based on domain similarity and content alignment.

Model Info:
Trained using Triplet Loss to optimize for semantic similarity.

Embeddings reflect both language context and domain-specific knowledge.

Output:
Each step of the pipeline saves an updated version of the file, using automated file naming (e.g. _top3, _chunks, _done).

Input Requirements:
.pdf,.docx,.txt,.xlsx,.xls

.csv file containing domain labels and associated terminology

