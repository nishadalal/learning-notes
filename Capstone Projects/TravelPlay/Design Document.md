---
title: "Capstone Project Design: TravelPlay"
description: "A personalized, AI-powered tool for creating travel activity books for kids"
tags: [capstone, design-doc, generative-ai, education, travel]
date: 2025-08-07
---

# 🎓 Capstone Project Design: **TravelPlay**

## 🧭 Goal
Design and build a generative AI web tool that enables parents to create **custom travel-themed activity worksheets** for children based on age, destination, and interests. The goal is to learn and demonstrate practical AI app-building skills, from prompting to deployment.

---

## 👥 Target Users

| User Type   | Description |
|-------------|-------------|
| 👨‍👩‍👧 Parents | Planning trips with kids (ages 3–12) |
| 🧑‍🏫 Educators | Teachers or homeschoolers looking for themed material |
| 🧒 Children | End users (passive) — content must be fun and age-appropriate |

---

## 🧩 Core Features

| Feature                        | Description                                                         |
| ------------------------------ | ------------------------------------------------------------------- |
| Input Form                     | Ask for destination, age, name, trip duration, interests optionally |
| Text Content Gen               | Use LLM to generate age-appropriate games, facts, quizzes           |
| Image Generation               | Use DALL·E or similar to generate illustrations                     |
| PDF Export                     | Bundle all content into a printable PDF                             |
| Embedding-based RAG (Optional) | Pull local/country data from embeddings                             |
| UI (Phase 2)                   | Streamlit or simple web form                                        |
| Shareable Output               | QR code or direct download for generated PDF                        |

---

## 🛠️ Tech Stack

| Layer        | Tools                                                                               |
| ------------ | ----------------------------------------------------------------------------------- |
| Prompting    | OpenAI GPT-4-turbo / Claude (for educational content)                               |
| PDF Export   | `fpdf2`, `reportlab`, or similar Python lib                                         |
| Image Gen    | DALL·E API (OpenAI)                                                                 |
| Backend      | Python script / FastAPI microservice (optional)                                     |
| UI (Phase 2) | Streamlit or Next.js (optional in Week 5+)                                          |
| Data         | Wikipedia (RAG), CSVs, scraped country/animal/flag data                             |
| Versioning   | Git + GitHub repo: [`learning-notes`](https://github.com/nishadalal/learning-notes) |
| Publishing   | Obsidian → Git → Quartz site → [nishadalal.com](https://nishadalal.com)             |

---

## 🧠 AI Skills & Learning Goals

- Prompt engineering (custom templates, chaining)
- Working with OpenAI APIs and streaming responses
- RAG pipeline: embeddings + retrieval
- Dynamic content generation + structured layout (PDF)
- Deploying functional, real-world AI tools
- Writing and reflecting via technical blogs

---

## 📐 Constraints

- PDF should be 5–10 pages max
- No login/auth in v1
- Lightweight interface (form + button)
- Cost-effective: < $20 total LLM/image API use
- Fun, clear UX for non-technical users

---

## 🔮 Stretch Goals

- Voice assistant (Whisper) to collect preferences
- Save session, regenerate activity sets
- Multilingual support
- PDF preview before download
- Shareable QR code or short link

---

## 🗓️ Timeline (Study Plan Alignment)

| Week | Focus |
|------|-------|
| ✅ Week 1 | Capstone scoping, learning pipeline, basic LLMs |
| 🔄 Week 2 | Prompting + PDF generation basics |
| Week 3 | Text content logic: quizzes, games, structure |
| Week 4 | Add image generation, improve layout |
| Week 5 | Build basic frontend (Streamlit) |
| Week 6 | RAG stretch: local country/animal/flag DB |
| Week 7 | Error handling, UX, testing |
| Week 8 | Final blog post + deploy

---

## 🧪 Deliverables

| Deliverable              | Description                                                                            |
| ------------------------ | -------------------------------------------------------------------------------------- |
| `capstone-design.md`     | This document                                                                          |
| `prompting-tests.ipynb`  | LLM content generation experiments                                                     |
| `worksheet-generator.py` | Core app logic to generate worksheet PDF                                               |
| `blog/`                  | Weekly learning blog posts on Quartz                                                   |
| `vault/`                 | Obsidian vault with Zettelkasten-style notes                                           |
| Public site              | Quartz-powered blog at `nishadalal.com`                                                |
| GitHub Repo              | [`learning-notes`](https://github.com/nishadalal/learning-notes) with synced structure |

---

## ✍️ Writing & Sharing

You'll also reflect weekly using:
- Obsidian Weekly Reflection Template
- Blog posts published every week

