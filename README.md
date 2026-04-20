Marketing Impact Copilot: AI Career Coaching Chatbot

 Overview
Navigating the expansive landscape of the marketing industry presents a significant challenge for early-career professionals and recent graduates. These individuals frequently encounter a lack of structured guidance regarding specific career trajectories, practical project execution, and the optimization of resumes for modern Applicant Tracking Systems (ATS). 

The Marketing Impact Copilot (Persona: "Smokey") is an AI-driven career coaching solution built to address this knowledge gap. Engineered using Microsoft Copilot Studio, Claude 3.1 Sonnet, and Google Gemini, this conversational platform provides highly tailored career advice, actionable portfolio blueprints, and ATS-optimized "XYZ" resume templates based on a rigorously structured dataset of 300+ marketing roles.

 Core Capabilities (The 3 Query Types)

Smokey is programmed to handle three primary user flows, strictly anchored to the uploaded CSV Knowledge Base to prevent AI hallucination:

Type A: Job Advice & Roadmaps**
    Provides realistic job advice, industry constraints, and career roadmaps based on the user's preferred domain (e.g., SEO, Product, Branding, FinTech, SaaS).
 Type B: Resume Rewriting (The XYZ Framework)**
    Translates weak, generic user task lists into polished, ATS-friendly content using the Google XYZ formula: *"Accomplished [X] as measured by [Y], by doing [Z]"*. It intelligently injects realistic placeholders and niche-specific keywords to elevate the professional narrative.
Type C: Portfolio Blueprints**
    Guides users away from basic, fluffy tasks (e.g., "managed social media") and generates highly actionable, constraint-based mock projects (Solo or Team). It details exact deliverables and primary KPIs to bridge the "experience gap" for freshers.

---

System Architecture & Data Flow

The system orchestrates a seamless flow between natural language understanding, database retrieval, and generative AI refinement.

```text
    ( START )  
        │
        ▼
  ╱ USER INPUTS QUERY ╱  ◄───────────────────────────────────────┐
 ╱ (e.g., "Need SEO Resume") ╱                                   │
        │                                                        │
        ▼                                                        │
┌─────────────────────────────────┐                              │
│ PROCESS: Copilot Studio parses  │                              │
│ Natural Language Intent & Data  │                              │
└─────────────────────────────────┘                              │
        │                                                        │
        ▼                                                        │
┌─────────────────────────────────┐                              │
│ PROCESS: Query CSV Database     │                              │
│ Extract Skills, Constraints,    │                              │
│ Projects, and specific KPIs     │                              │
└─────────────────────────────────┘                              │
        │                                                        │
        ▼                                                        │
┌─────────────────────────────────┐                              │
│ PROCESS: Construct System       │                              │
│ Prompt (Raw Data + User Intent) │                              │
└─────────────────────────────────┘                              │
        │                                                        │
        ▼                                                        │
┌─────────────────────────────────┐                              │
│ PROCESS: LLM (Claude/Gemini)    │                              │
│ applies XYZ formatting & tone   │                              │
└─────────────────────────────────┘                              │
        │                                                        │
        ▼                                                        │
  ╱ OUTPUT: Deliver Formatted  ╱                                 │
 ╱ Resume/Advice to User Chat ╱                                  │
        │                                                        │
        ▼                                                        │
      ╱ ╲                                                        │
    ╱     ╲                                                      │
  ╱ FOLLOW  ╲ ── YES ────────────────────────────────────────────┘
  ╲   UP?   ╱           
    ╲     ╱             
      ╲ ╱               
        │ NO
        ▼
     ( END )
