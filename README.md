# 🎶 Cover Identification System Using Lyrics Only 

## 📋 Project Overview

This project aims to build a system that takes a YouTube music video URL and returns the title and artist of the song by matching the lyrics with a database of songs. The goal is to identify potential cover songs by analyzing the lyrics. 

## 🛠️ Setup 
1. **Download a lyrics dataset.**
2. **Extract embeddings** for each song's lyrics using BERT.
3. **Create a vector index** (database) for fast retrieval of similar lyrics using FAISS.

## 🔍 Query Process For each YouTube URL (query): 
1. **Download** the YouTube video in a temporary file.
2. **Transcribe the lyrics** using the Insanely-fast-whisper model.
3. **Extract the embeddings** of the transcribed lyrics using BERT.
4. **Search the top-k similar entries** in your vector database using FAISS and return the song title and artist.

## 🔧 Tools and Technologies 
- **Insanely-fast-whisper** for transcribing lyrics.
- **BERT** for extracting embeddings.
- **FAISS** for creating a lyrics index and retrieving similar
