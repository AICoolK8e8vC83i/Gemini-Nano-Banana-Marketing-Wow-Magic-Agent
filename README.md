# AI Marketing Ad Generator (LangGraph + Gemini + ElevenLabs + FFmpeg)

## Overview
This project demonstrates an **end-to-end agentic pipeline** for automated ad generation, powered by state-of-the-art AI models and orchestration.  
The system is designed to **support marketing teams** by accelerating the creative process — not replacing human marketers, but giving them more time to focus on strategy and brand storytelling.

**Pipeline Features**
- **Prompt Enhancement** – Gemini 2.5 Flash improves base prompts with cinematic, high-detail ad styling.
- **Image Generation** – Gemini Nano Flash produces photorealistic visuals in multiple campaign styles.
- **Optional Image Editing** – Iterative refinement for fine-tuned campaigns.
- **Text-to-Speech (TTS)** – ElevenLabs generates natural-sounding, brand-ready voiceovers.
- **Video Assembly** – FFmpeg merges audio + visuals into final MP4 deliverables.
- **Multi-Ad Workflow** – Produces 5–8 variations in a single run, then concatenates into a final reel.

---

## Business Value
- **Accelerates Creative Workflows**: Cuts down ad production time from hours to minutes.  
- **Empowers Teams, Not Replaces Them**: Designed as a *co-pilot* for marketers and designers to experiment with ideas faster.  
- **Scalable A/B Testing**: Multiple ad variations per run → rapid iteration and campaign diversity.  
- **Cost-Efficient**: Streamlines parts of the pipeline while leaving room for human oversight and creativity.  
- **Enterprise Ready**: Flexible enough for agencies, startups, and global corporations.

---

## Technical Stack
- **LangGraph** – Agentic orchestration of multi-step workflows.  
- **Google Gemini 2.5 Flash** – Advanced prompt enhancement + image generation.  
- **ElevenLabs TTS** – High-quality voice synthesis for branding.  
- **FFmpeg** – Audio-visual merging and final video rendering.  
- **Python** – Modular, node-based architecture for extensibility.  

---

## Demo
- **YouTube Demo**: [Insert link here]  
- **Sample Outputs**: See `/demo/outputs/`

---

## How It Works
1. User provides a **base prompt** and optional style themes.  
2. Pipeline enhances the prompt, generates visuals, and synthesizes TTS.  
3. FFmpeg combines image + audio into standalone ad clips.  
4. Loop produces multiple variations, then concatenates them into a **final ad reel**.  

---

## Why This Matters
- **Human + AI Synergy**: Instead of automating away marketers, this tool acts as a *creative accelerator*, freeing teams to focus on storytelling, campaign strategy, and customer engagement.  
- **State-of-the-Art Technology**: Integrates cutting-edge models across vision, language, and speech to show what *agentic pipelines* can achieve in real business settings.  
- **Proof of Concept**: Demonstrates how enterprise marketing teams can adapt SOTA AI to gain **speed, scalability, and new creative dimensions**.  

---

## Setup
```bash
git clone https://github.com/your-username/ad-generator.git
cd ad-generator
pip install -r requirements.txt

**Create a .env file:**

GEMINI_API_KEY=your_key
ELEVEN_API_KEY=your_key

**Run:**

cd app

**Launch Gradio UI for interactive demo:**

python3 app.py
