# 5542SpeechSystem
# AI Speech Intelligence System for Meeting and Lecture Assistance

## Overview
This project is a speech intelligence system that converts audio from lectures / meetings into structured insights. The system uses a pretrained foundation model (Whisper) to transcribe speech and then applies a text analysis pipeline to generate summaries, action items, and keywords. The goal of this project is to show how modern foundation models can be used to build practical multimodal AI systems for productivity tasks.

---

## Features
- Speech-to-text transcription using Whisper
- Baseline summary generation
- Improved structured output
  - Summary
  - Action items
  - Keywords
- Comparison between baseline and improved outputs
- Evaluation across different audio conditions

---

## Project Pipeline

Audio Input  
↓  
Whisper Model (Speech-to-Text)  
↓  
Transcript  
↓  
Analysis Module  
↓  
Summary | Action Items | Keywords  

---

## Models Used

### 1. Whisper (openai/whisper-small)
- Pretrained speech recognition model
- Converts audio into text
- Handles different speech conditions (clean, noisy, fast speech)

### 2. Text Analysis Module
- Rule based processing system
- Extracts:
  - Summary
  - Action items
  - Keywords
- Designed to simulate structured output generation

---

## Dataset / Inputs

This project uses **custom-recorded audio samples** simulating real scenarios

- Clean lecture-style audio
- Meeting-style discussion audio
- Noisy audio recording
- Fast-paced lecture audio

These variations are used to evaluate system robustness under different conditions.

---

## How to Run

This project is designed to run in **Google Colab**.

### Steps:

1. Open the notebook:

2. Run all cells in order
- Install dependencies
- Load Whisper model
- Upload audio files when prompted

3. Upload your audio files (WAV/MP3 format)

4. The notebook will:
- Transcribe audio
- Generate baseline summary
- Generate improved structured outputs
- Save results to output files

---

## Outputs

For each audio file, the system produces

- Transcript
- Baseline summary
- Improved summary
- Action items
- Keywords
- Latency (processing time)

Outputs are saved as:
- `.txt` (transcripts)
- `.json` (structured results)
- `.csv` (evaluation table)

---

## Evaluation

The system is evaluated based on:

- Transcript quality
- Summary usefulness
- Action item relevance
- Keyword quality
- Latency

Different audio types (clean, noisy, fast, conversational) are used to analyze system performance under varying conditions.

---

## Results (Summary)

- High accuracy on clean lecture audio
- Strong action item extraction for audio
- Reduced performance in noisy conditions
- Improved structured outputs outperform baseline summaries

---

## Limitations

- Transcription accuracy decreases with noisy audio
- Overlapping speakers reduce performance
- Rule based extraction may miss complex action items
- Summary quality depends heavily on transcript quality
- No real time processing (batch-based system)

---

## Demo

Demo video link here


