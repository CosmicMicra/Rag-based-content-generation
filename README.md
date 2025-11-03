RAG + Gemini study Helper

Objective
To build an AI assistant that can analyze the transcript of any YouTube educational video, and automatically generate:

A detailed summary
- 10 flashcards for memory retention
- 10 MCQs to test understanding
- 5 external links to expand learning


📦 Install Required Libraries
We install necessary dependencies like:

google-genai for Gemini API access
youtube-transcript-api to extract transcripts
faiss-cpu and sentence-transformers for RAG

Summary of Key Concepts Used
This notebook uses several cutting-edge GenAI concepts:

1. Few-shot prompting: Guided the Gemini model with example outputs to generate structured summaries, flashcards, MCQs, and links from video transcripts.
2. Document understanding: Processed and analyzed YouTube video transcripts to extract key information for educational content creation.
3. Long context window: Enabled Gemini to handle large prompts, including few-shot examples and transcript chunks, for coherent content generation.
4. Gen AI evaluation: Assessed the quality of generated summaries, flashcards, and MCQs, likely through manual review, to ensure educational value.
5. Retrieval augmented generation (RAG): Retrieved relevant transcript chunks to enhance Gemini's generation of contextually accurate learning materials.
6. Vector search/vector store/vector database: Used FAISS to store and search transcript embeddings for efficient retrieval of relevant content.
7. Embeddings: Converted transcript chunks into semantic vectors using sentence-transformers to enable similarity-based retrieval for RAG.
