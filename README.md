# <img src="assets/germany-flag.svg" width="30" height="20" alt="German flag"> Amtly

### Germany, made simpler.

**Amtly** is an AI-powered assistant that helps people understand and navigate everyday formalities in Germany.

Moving to Germany, starting a new job, studying, dealing with health insurance, registering an address, understanding an official letter, or figuring out which authority to contact can be confusing — especially when you are new to the country.

Amtly turns a simple description of your situation into clear, actionable next steps.

---

## 💡 The Problem

German administrative processes can be difficult to navigate.

Users often need to:

- understand which authority is responsible
- find reliable information across multiple websites
- understand official German letters
- identify deadlines and required documents
- write formal replies
- understand which forms or applications they need
- navigate rules that depend on nationality, residence status, location, employment, or study status

For immigrants, language barriers make this even harder.

---

## 🚀 Our Solution

Instead of asking users to understand the system, **Amtly starts with their situation.**

For example:

> "I just moved from Ukraine to Hamburg and started a new job. What do I need to do?"

Amtly analyzes the user's context and provides:

- ✅ What needs to be done
- 🏢 Which authority or organization is responsible
- 📄 Which documents are required
- ⏰ Important deadlines
- 🔗 Relevant official sources
- ✉️ Help preparing letters or applications

---

## ✨ Core Features

### 💬 Ask Amtly

Describe your situation in your own words.

Examples:

> "I moved to another city. Where do I need to register?"

> "Can I use my Ukrainian driving licence in Germany?"

> "I started a new job. What do I need to do about health insurance?"

Amtly converts the situation into concrete next steps.

### 📄 Understand a Letter

Upload an official letter from, for example:

- Jobcenter
- Ausländerbehörde
- Finanzamt
- Krankenkasse
- Agentur für Arbeit
- local authorities

Amtly explains:

**What is this? → What do they want? → What is the deadline? → What should I do next?**

### ✍️ Prepare a Reply

Amtly can generate an appropriate German response based on the letter and the user's situation.

### 🏢 Find the Right Authority

Users don't need to know whether they need the Bürgeramt, Ausländerbehörde, Jobcenter, Krankenkasse, Finanzamt, or another organization.

They describe the problem — Amtly identifies where they need to go.

### 🌍 Multilingual Support

Users can communicate with Amtly in their preferred language while Amtly works with German official information and terminology.

### 🔐 Privacy First

Personal information from uploaded documents can be anonymized before being sent to an AI model.

---

## 🧠 How It Works

```text
                 User
                   │
                   ▼
              Amtly App
                   │
                   ▼
             User Context
                   │
                   ▼
              Anymize AI
          Personal Data Protection
                   │
                   ▼
               AI Agent
             OpenAI GPT
                   │
          ┌────────┴────────┐
          ▼                 ▼
    Official Sources    Document Analysis
          │
      Firecrawl
          │
          ▼
     Knowledge Base
          │
          ▼
       AI Reasoning
          │
          ▼
    Structured Response
          │
   ┌──────┼───────┐
   ▼      ▼       ▼
Explain  Actions  Reply
```

---

## 🛠️ Technology Stack

### OpenAI GPT

Main reasoning engine used for:

- understanding user situations
- document analysis
- multilingual interaction
- information synthesis
- generating letters and replies

### Firecrawl

Extracts structured, LLM-ready information from trusted German websites.

### Google Cloud / Vertex AI

Provides cloud infrastructure and can support the knowledge base, retrieval, and AI services.

### Anymize AI

Anonymizes sensitive information such as:

- names
- addresses
- IBANs
- insurance numbers
- case numbers
- dates

before documents are processed by AI.

### n8n

Connects the different components and orchestrates the Amtly workflows.

### Bilt

Used to rapidly build the user-facing application.

### ElevenLabs

Can provide voice interaction so users can talk to Amtly and listen to explanations.

---

## 🔎 RAG & Trusted Information

For administrative questions, reliability matters.

Amtly uses a Retrieval-Augmented Generation approach:

```text
User Question
      ↓
User Context
      ↓
Search Knowledge Base
      ↓
Retrieve Relevant Official Information
      ↓
AI Reasoning
      ↓
Answer + Source + Next Steps
```

The goal is to ground answers in trusted and official information rather than relying only on the model's internal knowledge.

---

## 👤 Personalized Context

Administrative requirements depend on the person.

Amtly can take context into account such as:

```text
Country of origin
Current city
Residence status
Employment status
Student status
Health insurance
Driving licence
Preferred language
```

This allows Amtly to provide situation-specific guidance instead of generic search results.

---

## 🎯 Example Use Cases

**Immigration**

> "I arrived from Ukraine. What do I need to do first?"

**Driving licence**

> "Is my Ukrainian driving licence valid in Germany?"

**Health insurance**

> "I started working in Germany. How do I get health insurance?"

**Moving**

> "I moved from Hannover to Hamburg. What do I need to change?"

**Official letter**

> "I received this letter from Jobcenter. What do they want from me?"

**Finding an authority**

> "I lost my residence permit. Where should I go?"

**Urgent situation**

> "I need medical help but don't know whom to contact."

---

## 🧪 Hackathon MVP

For the first prototype, Amtly focuses on four core workflows:

1. **Ask about a personal situation**
2. **Analyze an official letter**
3. **Find the responsible authority**
4. **Prepare a response**

Initial domains include:

- Immigration
- Health insurance
- Driving licences
- Everyday administrative formalities

---

## 🎯 Our Mission

People shouldn't need to understand an entire administrative system just to understand what they need to do next.

**Describe your situation. Understand your options. Take the next step.**

# Amtly — Germany, made simpler. <img src="assets/germany-flag.svg" width="30" height="20" alt="German flag">
