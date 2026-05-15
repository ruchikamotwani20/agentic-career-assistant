# AI Career Conversation Assistant

An AI-powered conversational portfolio assistant built using DeepSeek LLM APIs, Gradio, Hugging Face Spaces, and tool-calling workflows to enable context-aware career conversations, real-time interaction, and foundational AI agent behavior.

---

# Overview

This project was built to explore how modern AI applications are engineered beyond traditional chatbot interfaces.

The assistant acts as an interactive AI-powered version of my portfolio capable of answering questions about:

* Professional experience
* Technical skills
* Analytics engineering work
* AI and machine learning projects
* Research publications
* Career interests
* Data science workflows
* Operational analytics systems
* Agentic AI experimentation

The system dynamically loads contextual information from my LinkedIn profile and custom summary files, injects that context into the LLM prompt, and generates personalized responses in real time.

In addition to conversational interaction, the project also explores foundational concepts behind modern AI agents through function/tool-calling workflows, external system interaction, and workflow orchestration.

---

# Why I Built This

As someone deeply interested in AI systems, analytics engineering, operational automation, and modern LLM workflows, I wanted to move beyond simple notebook experimentation and build a deployable AI application that demonstrates how real-world conversational AI systems are structured.

This project became a hands-on exploration into:

* LLM application engineering
* Prompt engineering
* Context injection
* AI agent workflows
* Function/tool calling
* Workflow orchestration
* Deployment pipelines
* Conversational interfaces
* Real-world AI system architecture

One of the biggest takeaways from building this project was realizing how much modern AI applications rely not only on models themselves, but also on orchestration layers, context management, tooling systems, external integrations, and deployment infrastructure.

---

# Key Features

## Conversational AI Assistant

Built a real-time AI-powered conversational assistant capable of answering personalized questions related to my projects, experience, skills, and technical background.

---

## Context-Aware Responses

The assistant dynamically loads:

* LinkedIn profile data (PDF ingestion)
* Custom professional summary files

These are injected into the system prompt to provide contextual grounding for responses.

---

## Tool / Function Calling Workflows

Implemented OpenAI-style function calling workflows allowing the LLM to interact with external systems.

Current tools include:

* Recording user contact information
* Logging unanswered or unknown questions
* Triggering external push notifications

This introduces foundational AI-agent style behavior where the model can initiate actions rather than only generate text.

---

## Real-Time Push Notifications

Integrated Pushover APIs to send real-time notifications whenever:

* a user shares contact information
* the assistant encounters unknown questions

This demonstrates external workflow integration and real-world event handling.

---

## Hugging Face Deployment

The project is publicly deployed using Hugging Face Spaces with a Gradio-based frontend interface.

This transforms the project from a local prototype into a fully accessible web-based AI application.

---

## Modular Architecture

The codebase is intentionally structured to separate:

* prompt engineering
* context loading
* tool handling
* UI interaction
* deployment workflows

making the project easier to extend into larger AI-agent systems later.

---

# System Architecture

```text
User Input
    ↓
Gradio Chat Interface
    ↓
Python Backend (app.py)
    ↓
DeepSeek LLM API
    ↓
System Prompt + Context Injection
    ↓
Tool Calling Layer
    ↓
External Actions / Notifications
    ↓
Response Returned to User
```

---

# Tech Stack

## Languages & Frameworks

* Python
* Gradio

## AI / LLM

* DeepSeek APIs
* OpenAI SDK

## Context & Data Handling

* PyPDF
* JSON
* dotenv

## External Integrations

* Pushover API
* Requests Library

## Deployment

* Hugging Face Spaces

---

# Core AI Concepts Explored

This project explores several foundational concepts in modern AI engineering:

* LLM Application Development
* Prompt Engineering
* Context Engineering
* Tool / Function Calling
* AI Agent Foundations
* Conversational Orchestration
* External Workflow Integration
* Real-Time Deployment
* Dynamic Knowledge Injection
* Human-AI Interaction Design

---

# Project Structure

```bash
ai-career-conversation-assistant/
│
├── app.py
├── README.md
├── requirements.txt
├── .gitignore
│
├── Notebooks/
│   └── 4_lab4.ipynb
│
└── me/
    ├── linkedin.pdf
    └── summary.txt
```

---

# How It Works

## 1. Context Loading

At startup, the system:

* loads LinkedIn profile data from PDF
* loads custom summary text
* stores contextual information inside the assistant object

This contextual information becomes part of the system prompt.

---

## 2. System Prompt Construction

The application dynamically builds a system prompt instructing the model to:

* behave as a professional AI representation of me
* answer questions using provided context
* engage naturally with users
* use tools whenever appropriate

---

## 3. Conversational Workflow

When a user sends a message:

1. User message is received via Gradio
2. Context + conversation history are assembled
3. DeepSeek LLM API is called
4. Model generates response or requests tool usage
5. Python backend executes requested tools
6. Tool results are returned to the model
7. Final response is displayed in chat

---

## 4. Tool Calling Workflow

The assistant supports OpenAI-style tool/function calling.

Example behaviors include:

* collecting user email information
* logging unknown questions
* triggering notification workflows

This introduces basic AI-agent style orchestration.

---

# Deployment

The project is deployed publicly using Hugging Face Spaces.

Frontend:

* Gradio Chat Interface

Backend:

* Python + DeepSeek APIs

Hosting:

* Hugging Face Spaces

---

# Live Demo

Try the project here:

https://huggingface.co/spaces/ruchikamotwani20/Career_Conversation

---

# Future Improvements

Planned future enhancements include:

* Retrieval-Augmented Generation (RAG)
* Vector database integration
* Persistent conversational memory
* Multi-agent orchestration systems
* Voice interaction workflows
* Advanced evaluation pipelines
* Conversation analytics dashboard
* Tool-routing optimization
* Personalized recommendation workflows
* Autonomous workflow execution

---

# Author

Ruchika Motwani
MS Information Studies (Data Science & Analytics)
The University of Texas at Austin

Follow And Connect With Me on LinkedIn:
https://www.linkedin.com/in/ruchika-motwani/

---
