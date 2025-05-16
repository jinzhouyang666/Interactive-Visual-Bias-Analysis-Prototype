
# 🧠 Interactive Visual Bias Analysis Prototype

This repository contains a research prototype exploring how human feedback can guide AI models in recognizing and adapting to representational bias in cultural heritage imagery. Inspired by RLHF (Reinforcement Learning from Human Feedback) and DPO (Direct Preference Optimization), this project simulates personalized human-AI interaction without relying on predefined labels.

## 📚 Context & Motivation

AI models used in cultural institutions rely on demographic or visual labels that are often incomplete, ethically problematic, or biased. This project addresses the need for a more subjective and contextual learning framework by integrating multiple annotation sources and simulating user preferences.

The goal is to prototype a system where:
- Visual-language models (VLMs) generate descriptions of heritage images.
- User provides feedback about whether those descriptions capture issues of representation and bias.
- The model learns to adapt based on this interaction loop.

## 🖼️ Dataset

Images are retrieved from the [Rijksmuseum](https://www.rijksmuseum.nl) using culturally sensitive search keywords (e.g., "colonial", "Asian woman", "Black servant"). Each image includes:

- Institutional Dutch-language metadata
- Machine-generated annotations (via Encord and LLaMA-4)
- Simulated human feedback from two different perspectives
- A structured bias divergence analysis
- A pairwise human preference dataset to simulate RLHF-style learning

## 🧩 Key Components

- `notebooks/`: Colab-style notebook with full demo and analysis
- `interactive_feedback_flowchart.png`: Conceptual diagram of the interactive learning system
- `data/annotations.csv`: Structured comparison of human and AI annotations
- `data/preferences.csv`: Pairwise human feedback preferences for RLHF/DPO simulation

This prototype was developed to explore bias mitigation and personalization methods in human-AI interaction for cultural heritage. It offers a practical demonstration of methodological contributions in the intersection of:

- Bias-aware AI
- Vision-language systems
- Human-in-the-loop personalization
