# Joseph — AI Job Hunting Pipeline

> "Like the biblical Joseph, his job is to read the signs and help me prepare."

A personal 6-agent AI pipeline that automates daily job research — cutting
manual research from 3–4 hours per application to under 20 minutes per day.

![Joseph dashboard showing job pipeline output](/dashboard-preview.png)


## The problem

Applying for software roles manually takes 3–4 hours per job: discovery,
filtering, reading JDs, company research, gap analysis, cover letter. That
block of time rarely exists all at once, so applications stall.

## The solution

Six specialised AI agents run automatically each morning and deliver
structured results to Telegram.

| Agent | Role |
|---|---|
| 🔍 Scraper | Discovers new listings from public job boards |
| 🚫 Filter | Removes mismatched roles (senior titles, clearance requirements) |
| 📋 Qualifier | Reads each full JD for a deeper second-pass assessment |
| 🏢 Researcher | Finds company size, tech stack, commute time, team data |
| 📊 Gap Analyser | Compares resume against JD and surfaces real skill gaps |
| ✍️ Adviser | Drafts a tailored cover letter using actual company context |


## How It Works

![Joseph architecture](/joseph_job_agent_architecture.png)


## Architecture evolution

**v1 — Python / Claude Code**  
Built over Easter 2026. Six agents coded in Python, orchestrated via
Claude Code, delivering Telegram notifications per qualifying role.

**v2 — Claude Cowork migration**  
Migrated the agent pipeline to Claude Cowork for token efficiency and
context management. Added a live HTML dashboard to monitor job market
activity, track evaluated roles, and visualise pipeline output in real time.

## Tech stack
- v1: Python, Claude Code, Anthropic API, Telegram Bot API
- v2: Claude Cowork (Anthropic Agent SDK), HTML/JS live dashboard, JSON store

## Outcomes
- 3–4 hrs/application → under 20 min/day
- 300+ roles evaluated, scored, and logged with gap analysis

---
*Pipeline is private (personalised data). This repo documents the architecture.*
