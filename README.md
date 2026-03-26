# AI Email Content Generator (MQL vs Subscriber Targeting)

## Overview

This project is an automated email content generation system that creates high-quality, research-backed email copy based on user inputs from Google Sheets.

It differentiates messaging for Market Qualified Leads (MQLs) and Subscribers, ensuring tailored communication for different stages of the funnel.

## Problem

Writing effective email copy at scale is challenging because:

It requires research-backed context
Messaging differs across funnel stages (MQL vs Subscriber)
Manual writing is time-consuming and inconsistent
Maintaining quality across campaigns is difficult

## Solution

This system automates the entire workflow:

User inputs a prompt in Google Sheets
Selects target audience (MQL or Subscriber)
AI researches the topic using Perplexity AI
Generates email copy using OpenAI models
Validates and refines output via Claude
Outputs final copy into Google Docs and updates the sheet

## How It Works
User Input (Google Sheets)
        ↓
Router (Audience Type: MQL vs Subscriber)
        ↓
Research Layer (Perplexity AI)
        ↓
Content Generation (OpenAI)
        ↓
Quality Check (Claude)
        ↓
## Output:
   → Google Docs (Email Copy)
   → Google Sheets (Status Update)

## Tech Stack
Make (Integromat) – Workflow orchestration
Google Sheets – Input & tracking
Google Docs – Output storage
Perplexity AI – Research layer
OpenAI – Content generation
Claude – Validation & refinement

## Key Features

✅ Audience-based content routing (MQL vs Subscriber)
✅ Automated research before generation
✅ Multi-model AI pipeline (generation + validation)
✅ Structured output storage in Google Docs
✅ Scalable content generation via spreadsheet interface
## Workflow Logic
1. Input Layer

User provides:

Prompt/topic
Audience type (MQL or Subscriber)
2. Research Layer
Perplexity AI gathers relevant context and insights
3. Content Generation
OpenAI generates initial email draft tailored to audience
4. Validation Layer
Claude checks:
clarity
tone
relevance
coherence

5. Output Layer
Final email stored in Google Docs
Status and links updated in Google Sheets

 ## Use Cases
B2B outbound campaigns
Lead nurturing sequences
Newsletter content generation
Marketing automation workflows
Personalized email campaigns at scale

## Routing Logic
If Audience = MQL
   → More direct, conversion-focused messaging

If Audience = Subscriber
   → Educational, value-driven messaging

## Example Flow
User enters:
“Write an email about AI automation for recruitment agencies”
Selects: MQL
System:
researches topic
generates targeted email
refines output
Final email appears in Google Docs

## Limitations
Output quality depends on prompt clarity
Requires API access to AI tools
May require prompt tuning for niche industries
## Future Improvements
Add personalization variables (name, company, industry)
Integrate with email sending tools (e.g., SMTP/CRM)
Add A/B testing for subject lines
Include performance tracking (open rates, CTR)
## Author Notes

This project demonstrates how multiple AI systems can be orchestrated into a single automated content pipeline, combining:

research
generation
validation

to produce high-quality, context-aware email copy at scale.
