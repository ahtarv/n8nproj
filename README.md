# 🎬 AI Content Experimentation Studio (n8n)

**Rapidly generate, iterate, and A/B test short-form video content** — scripts, hooks, captions, and more — using AI + automation.

Built with **n8n**, this system removes the repetitive brainstorming & rewriting drudgery so creators, marketers, and teams can run many more creative experiments in far less time.

[![n8n](https://img.shields.io/badge/automation-n8n-00A86B?style=flat&logo=n8n)](https://n8n.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![AI Powered](https://img.shields.io/badge/AI-powered-🔥-purple)](https://github.com/yourusername/ai-content-studio)

## ✨ Why This Project Exists

Content creators waste **hours** every week on:

- Coming up with fresh hooks
- Rewriting the same script 5–10 times
- Crafting 20 caption variations
- Trying different tones (funny, inspirational, sarcastic…)

This system **automates the boring 70%** so you can focus on the fun 30%: storytelling, filming, and analyzing what actually performs.

**Goal**: 10× faster experimentation without losing human creative control.

## 🌟 Features

- Generate **3–10 variants** of hooks, scripts & captions from one idea
- Control **tone**, **emotion**, **length**, **format** via simple parameters
- Auto-tag outputs (e.g. `motivational`, `storytelling`, `question-hook`, `listicle`)
- Structured JSON + readable Markdown outputs ready for copy-paste
- Human-in-the-loop: review & pick winners before posting
- Pluggable storage: local files, Notion, Google Sheets, Airtable…

## 📊 Example Output

Input prompt:  
"Productivity tip about beating morning procrastination"

**Hook options**  
1. "I used to lose 90 minutes every morning… until I discovered this 17-second trick"  
2. "The brutal truth: your morning routine is killing your productivity"  
3. "Question: Are you secretly sabotaging your day before 9 AM?"

**Script variations** (30–60 sec formats)  
- Storytelling version  
- List format (3 reasons + fix)  
- Contrarian / myth-busting angle

**Caption styles**  
- Emoji-heavy & punchy  
- Thoughtful & reflective  
- Call-to-action strong  
- Thread-style carousel teaser

All tagged:  
`tone: motivational | format: question-hook | emotion: relatable | length: short`

## 🚀 Quick Start

1. Have **n8n** running (self-hosted recommended)  
   → [Quick install guide](https://docs.n8n.io/hosting/installation/)

2. Import the workflow  
   → Download [`content-experiment-workflow.json`](./workflows/content-experiment-workflow.json)  
   → n8n → **Import from File** or **Import from URL**

3. Configure credentials  
   → Add your LLM API key (OpenAI, Anthropic, Groq, Gemini…)  
   → Optional: Notion / Google Sheets integration

4. Run it!  
   → Manual trigger → enter your idea + parameters  
   → Watch variants appear in seconds

## 🛠️ Current Capabilities (v1.0)

- Manual trigger (one idea at a time)
- Text-only generation (hooks, scripts, captions)
- Variant diversity via prompt engineering
- Basic tagging logic
- Output to local disk / Notion

**No auto-posting** — human always decides what goes live.

## 🔮 Roadmap & Possible Extensions

- [ ] Schedule + batch processing (10 ideas from Google Sheet)
- [ ] Auto-format per platform (TikTok vs Reels vs Shorts vs X)
- [ ] Performance feedback loop (pull views/likes → feed back to prompts)
- [ ] Auto-posting (Instagram, YouTube Shorts, TikTok, X) – with approval step
- [ ] A/B testing helper (generate thumbnail text + caption pairs)
- [ ] Voiceover script variant + ElevenLabs integration
- [ ] Multi-LLM comparison mode (same prompt → see which model wins)

## 🧩 Tech Stack

- **Core**: n8n (self-hosted)
- **AI**: Any OpenAI-compatible LLM (Claude, Gemini, Llama 3 via Groq/Ollama…)
- **Data**: JSON + Markdown
- **Optional destinations**: Notion, Google Sheets, Airtable, Supabase, files

## 🙌 Contributing

Ideas, bug fixes, new prompt templates, storage nodes, or platform formatters are very welcome!

1. Fork & branch (`feat/amazing-new-variant-generator`)
2. Add / improve
3. Open PR with clear description

Even small things help: better prompt examples, UI screenshots, or workflow diagram updates.

## ⚖️ License

MIT – do whatever you want with it.  
Just don't blame me if your content goes mega-viral and you become too famous 😄

Made with ❤️ for creators who love to experiment.
