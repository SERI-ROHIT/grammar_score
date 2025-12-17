#  Grammar Scoring Engine from Voice Samples
Overview

This project implements a Grammar Scoring Engine that evaluates spoken English audio samples and predicts a grammar quality score.
The system converts speech to text and analyzes grammatical correctness using NLP-based techniques.

This solution was developed as part of the SHL Research Intern Assessment (Option 2).

Problem Statement

Given an audio recording of spoken English, the task is to:

1. Convert speech into text

2. Analyze grammatical quality of the text

3. Generate a grammar score reflecting accuracy and clarity

##  Approach & Architecture
Audio Input (.mp3)
        ↓
Audio Preprocessing (Noise Reduction)
        ↓
Speech-to-Text (OpenAI Whisper)
        ↓
Text Cleaning & Normalization
        ↓
Grammar Analysis (LanguageTool)
        ↓
Feature Extraction
        ↓
Grammar Scoring

## Tools & Technologies Used

Audio Processing-	librosa, noisereduce

Speech-to-Text-	OpenAI Whisper

Grammar Checking-	language-tool-python

Text Analysis	textstat- regex

Machine Learning (Optional)-	scikit-learn

Language	Python- 3.10

## Grammar Scoring Logic

A rule-based scoring approach is applied:

Higher grammar errors → lower score

Better readability → higher score

Score Range:

1 → Poor grammar

5 → Excellent grammar

example--

{
  "audio_file": "download_mp3.mp3",
  "grammar_errors": 2,
  "grammar_score": 3.6
}



## Conclusion

This project demonstrates a practical, scalable, and explainable grammar assessment system using speech processing and NLP techniques.
The approach aligns with real-world assessment platforms and is suitable for automated language evaluation use cases.
