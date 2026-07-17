# Zenith-Style-Assistant-Claude-Artifact-Prototype-
# 🎨 Zenith Style Assistant

A six-question style quiz that merges **seasonal colour analysis** and **generative outfit styling** into a single, one-shot Claude API call.

-**https://claude.ai/public/artifacts/6e1a02cf-bff6-436d-b651-fa76da919be9**` – Fully self-contained UI (HTML/CSS/JS) built to run as a Claude.ai Artifact.
- **`prompt-engineering-breakdown.pdf`** – The exact system prompt used, plus annotated design decisions (JSON schema, tonal guardrails, and edge-case handling).

## 🔍 What makes this prompt engineering different
- **Fixed JSON schema** (6 best colors, 3 to avoid, 3 outfits) keeps the UI grid perfectly stable.
- **Constructive avoidance** – never calls a color "bad"; always frames it as "save for accessories."
- **Forced confidence** – the AI must make a decisive call even if the user says "unsure" about their undertone.
- **Brand voice lock** – styled as a "confident, warm older sibling," never a clinical beauty lecture.

## ⚠️ Important: Running this locally
This prototype is **engineered for the Claude.ai Artifact sandbox**, where the Anthropic API key is automatically injected.

**If you open `index.html` directly in your browser**, the API call will fail (CORS + missing auth). To make it standalone, you'd need to add a backend proxy (e.g., Vercel/Netlify function) to hold your API key.

This repo is a **prompt-engineering + UI portfolio piece**, not a production web app.

---
*Built as part of a design & AI assignment for Zenith.*
