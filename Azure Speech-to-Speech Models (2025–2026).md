Azure Speech-to-Speech Models (2025–2026)


Here's the complete picture of what's available, organized by how they work:

The main Speech-to-Speech platform: Azure Voice Live API
Voice Live API is a unified single API for real-time speech-to-speech conversations, allowing developers to build voice assistants, agents, and chatbots. It has been generally available since Ignite 2025 with 10+ natively integrated GenAI models. Microsoft Community Hub It replaces the old approach of manually chaining STT → LLM → TTS yourself.

Real-time S2S models (native audio in → audio out)
These models handle the full conversation loop with no intermediate text step:
gpt-realtime-mini (version 2025-12-15) and gpt-realtime-1.5 (version 2026-02-23) are the current real-time models. The Realtime API supports up to 32,000 input tokens and 4,096 output tokens. Microsoft Learn
The gpt-realtime-mini-2025-12-15 model delivers improved prosody, better voice fidelity across turns, and reduced latency — ideal for low-latency, high-quality voice experiences. Microsoft Community Hub
phi4-mm-realtime is Microsoft's own multimodal model that supports native audio in/out and is optimized for edge or in-car assistant scenarios. Microsoft Learn

GPT models used inside Voice Live (Azure Speech handles STT/TTS)
Voice Live supports GPT-5, GPT-4.1, GPT-4o, Phi, and more — with different models offering different levels of intelligence, speed, latency, and cost. Microsoft Learn For these models, Azure Speech Service handles the voice input and output while the GPT model handles the reasoning.

Three pricing tiers inside Voice Live
Voice Live Pro lets you choose from GPT-4o-Realtime, GPT-4o, and GPT-4.1. Voice Live Basic covers GPT-4o-Mini-Realtime, GPT-4o Mini, and GPT-4.1 Mini. Voice Live Lite covers SLMs and Phi models including GPT-4.1 Nano. Microsoft Community Hub

Speech input (STT) options
Azure Speech-to-Text offers real-time transcription, fast transcription, batch transcription, and an LLM Speech preview that transcribes and translates using LLM-enhanced models with prompt tuning support. Azure It covers 140+ languages.

Voice output (TTS) options
You can select from hundreds of natural multilingual voices including the latest HD V2 neural voices across 150+ locales, and also use custom voice to create brand-specific voices. Microsoft Community Hub
For the Indian market specifically, Aarti (female) and Arjun (male) are natural conversational voices trained with professional voice artists, ideal for customer support and digital assistants in Hindi and English. 
