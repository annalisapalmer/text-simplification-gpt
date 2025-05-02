## Summary: Exploring Text Simplification

This project replicates and extends several strategies for text simplification:

### Manual and Rule-Based Methods

- Defined manual simplifications for philosophical and historical excerpts.
- Applied readability scoring (Flesch Reading Ease, Grade Level) to confirm simplification success.
- Built a synonym replacement tool using WordNet and n-gram frequency analysis to replace complex words with simpler, more common equivalents.

### Embedding and Similarity

- Used `text-embedding-ada-002` to generate sentence embeddings.
- Measured cosine similarity between complex and simplified sentences to assess meaning preservation.

### GPT-Based Prompting

- Zero-shot: Given a single sentence, GPT rewrote it using simpler vocabulary.
- Few-shot: Provided 4–5 paired examples to fine-tune GPT’s responses contextually.
- Prompt variations were created to modulate the level of simplification.

### Evaluation

- Visualized complexity reduction with readability plots.
- Logged semantic similarity scores across simplification techniques.

## Key Insights

- GPT-3 is highly effective at semantic simplification but can occasionally "hallucinate."
- Heuristic synonym replacement is limited but interpretable.
- Readability metrics do not always correlate with human-perceived simplicity.

## Next Steps

- Extend this work using fine-tuned models on larger simplification datasets (e.g., WikiLarge).
- Introduce context-aware simplification that accounts for downstream tasks like summarization or translation.
