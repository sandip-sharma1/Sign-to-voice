# Symbol-to-Voice: A Multimodal System for Symbol Recognition and Speech Generation

A multimodal system that converts visual symbols or gestures into natural human speech, enabling assistive communication with multilingual support (English and Nepali).

## Overview

Symbol-to-Voice is an early-stage research project that integrates computer vision techniques for symbol recognition with neural text-to-speech (TTS) models for speech generation. The system aims to interpret input symbols and convert them into intelligible speech in multiple languages, supporting accessibility for individuals with speech or hearing impairments.

## Problem Statement

Existing communication systems for symbol or gesture interpretation are limited to text output or single-language support. This project addresses the need for:

- Accurate visual symbol and gesture recognition
- Conversion to meaningful text
- Natural speech generation in multiple languages
- Scalable assistive communication

## System Architecture

**Two-stage pipeline:**

1. **Visual Recognition Module**: CNN-based feature extraction and classification of input symbols/gestures
2. **Speech Synthesis Module**: Neural TTS (FastSpeech2) converts classified output to speech in multiple languages

**Architecture Flow:**

```
Input (Symbol / Gesture Image)
        ↓
Preprocessing (Normalization, Resizing)
        ↓
CNN-Based Feature Extraction
        ↓
Symbol Classification
        ↓
Text Mapping Layer
        ↓
Language Selection Module
        ↓
FastSpeech2 TTS Model
        ↓
Speech Output (Audio)
```

## Key Technologies

- **CNN**: For feature extraction and symbol classification
- **FastSpeech2**: For neural text-to-speech generation
- **Multimodal Learning**: Combines vision and speech synthesis
- **Multilingual Support**: English and Nepali TTS

## Current Work Stage

The project is in the initial research and design phase:
- Literature review of symbol recognition and TTS systems
- Identification of suitable CNN architectures
- Study of FastSpeech2 and related speech synthesis models
- Dataset exploration for symbols and multilingual speech
- System design and pipeline definition

## Future Scope

- Real-time symbol recognition using camera input
- Support for continuous gesture and sign language recognition
- Improved low-resource language support (Nepali TTS enhancement)
- Deployment as a web or mobile-based assistive system
- End-to-end optimization for real-time inference

## References

- https://ijnrd.org/papers/IJNRD2307387.pdf
- https://arxiv.org/abs/1901.05613