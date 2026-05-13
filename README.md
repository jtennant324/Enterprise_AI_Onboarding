> **Demo notice:** This is a portfolio project intended for demonstration purposes only. Do not enter sensitive, confidential, or personally identifiable information. API keys are not stored but are held in browser memory for the duration of your session.

# Enterprise AI Onboarding Tool

An interactive onboarding assistant that helps everyday office workers understand how to use Claude AI productively and safely at work, with no technical background required.

**Live demo:** https://jtennant324.github.io/Enterprise_AI_Onboarding/

---

## YouTube Demo Video

<a href="https://youtu.be/e9hdBBGZ7lw">
  <img src="https://img.youtube.com/vi/e9hdBBGZ7lw/maxresdefault.jpg" width="400" alt="Demo Video" />
</a>

## What it does

This tool is designed for anyone stepping into an AI-enabled workplace for the first time, from entry-level staff to executives. It answers common questions about enterprise AI use in plain language, without jargon or assumed technical knowledge.

Users can:
- Click pre-built topic cards covering the most common onboarding questions
- Ask their own questions in a free-text chat interface
- Follow clickable suggested questions at the end of each response to continue exploring

Responses are formatted for readability using bullet points, bolded key ideas, and short paragraphs. Every response also ends with suggested next questions to help users who are unsure what to ask next.

---

## What it demonstrates

- **Prompt engineering** - a carefully designed system prompt that controls tone, format, structure, and response behavior for a non-technical audience
- **Anthropic Claude API integration** - real-time API calls using the `/v1/messages` endpoint, with conversation history maintained across the session
- **CORS-safe architecture** - API requests are routed through a Cloudflare Worker to prevent browser security issues while keeping the API key out of client-side code
- **Markdown rendering** - assistant responses are parsed and rendered as formatted HTML using marked.js
- **Clickable follow-up questions** - dynamically generated numbered lists become interactive so users can continue exploring without typing
- **Enterprise AI awareness** - built-in privacy guidance for topics involving HIPAA, PII, credentials, and confidential data

---

## How to run it locally

1. Clone the repo
2. Open `index.html` using a local server (VS Code Live Server works well)
3. Enter your Anthropic API key when prompted: https://console.anthropic.com
4. Your key is never stored and exists only in memory during the current session

> Note: Opening `index.html` directly as a `file://` URL will not work because of browser CORS restrictions. Use a local server instead.

---

## Tech stack

- HTML, CSS, JavaScript (vanilla, no frameworks)
- Anthropic Claude API (`claude-sonnet-4-5`)
- Cloudflare Workers (API proxy)
- marked.js (markdown rendering)
- Hosted on GitHub Pages

---

## Project context

Built as part of a portfolio demonstrating hands-on experience with enterprise AI integration, prompt engineering, and AI governance concepts. Designed with the end user in mind, especially non-technical coworkers who may need additional support as AI tools are introduced into the workplace.
