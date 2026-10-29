# Sachin Shinde — HR Product Manager & Job Outreach Agent Plugin

A specialized agent and skill plugin designed to represent **Sachin Shinde** in product management job applications, recruitment communications, and networking outreach.

---

## Overview

This plugin turns Antigravity into an intelligent, honest, and high-converting Career and Outreach Agent. It analyzes job descriptions, performs objective fitment scoring against Sachin's verified CV, discovers relevant hiring contacts, and crafts concise, high-converting outreach messages tailored to each channel.

### Key Capabilities
- **JD Intake & Executive Summary**: Structured intake checklist highlighting mandatory requirements, scope, and location parameters.
- **Visual Fit Score Scorecard**: Executive callout banner featuring an ASCII/block progress meter, a 4-dimension alignment breakdown, and a clear win-condition thesis.
- **Strategic Alignment Section**: 
  - 📊 Multi-dimensional alignment scorecard with match quality badges.
  - 🏛️ The Three Strategic Alignment Pillars mapping role needs to quantifiable outcomes.
  - ⚖️ Transparent gap analysis and transferable bridge strategies.
- **People Targeting Workflow**: Surfaces hiring managers, team leads, and recruiters via structured public search queries with confidence scores.
- **Tailored Outreach Generation**:
  - **LinkedIn Connection Notes**: Strictly under 300 characters.
  - **LinkedIn InMails**: Focused pitch under 150 words with low-friction CTAs.
  - **Referral Emails**: Under 150 words with an immediate forwardable 3rd-person blurb.
  - **Direct Hiring Manager Pitches**: Problem-led emails addressing specific domain pain points.

---

## Operating Invariants

1. **Zero Hallucination**: Every claim, metric, tool, and achievement is drawn directly from Sachin's verified CV. No inflated metrics, fictional team sizes, or imaginary domain experience.
2. **Strict Privacy**: Never outputs Aadhaar, PAN, RRN, passport, or government identification numbers. Verification journeys are referenced strictly by flow name.
3. **Peer-to-Peer Tone**: PM-to-PM communication. Direct, outcome-driven, and free of AI clichés ("thrilled", "unique positioning", "passionate about").
4. **Hard Limits Enforced**: LinkedIn notes are strictly < 300 characters; InMails and referral emails are strictly < 150 words.
5. **Immediate Joiner Priority**: All outreach messages, notes, and emails explicitly highlight that Sachin is an immediate joiner (0-day notice period) so that his profile is prioritized.
6. **Pune Location Advantage**: Explicitly highlights that Sachin is already based out of Pune whenever the role or company is located in Pune.
7. **Clean Copy Boxes**: Character counts and word counts are placed outside the code blocks so users can copy clean message text directly.
8. **Direct Mobile Reachout**: Sachin's mobile number (`+91 8149408727`) is included in sign-offs and contact lines for fast reachout.
9. **Visual Hierarchy & Rich Scorecards**: Displays prominent executive callouts with progress bars, 4-pillar dimensional grids, and clean metadata cards below every copy box.

---

## Available Commands

| Command | Description |
|---|---|
| `/analyze-jd` | Evaluates a job description, displays visual scorecard, alignment pillars, and highlights gaps. |
| `/find-people` | Finds target hiring managers, recruiters, and product leaders for a job posting. |
| `/connection-note` | Crafts a concise LinkedIn connection invite (< 300 chars). |
| `/inmail` | Drafts a punchy LinkedIn InMail (< 150 words) with a 10-minute chat ask. |
| `/referral-email` | Drafts a referral request with a self-contained 3rd-person forwardable blurb. |
| `/hiring-manager-email` | Drafts a problem-focused direct pitch to the hiring manager. |
| `/full-outreach` | Generates the entire outreach pack in one structured response. |

---

## Plugin Structure

```text
~/.gemini/config/plugins/sachin-career-agent/
├── plugin.json                                # Plugin manifest
├── README.md                                  # User documentation
├── rules/
│   └── AGENTS.md                              # Always-on operating and tone rules
├── agents/
│   └── sachin-career-agent.md                 # Dedicated Career & Outreach subagent
└── skills/
    └── sachin-job-outreach/
        ├── SKILL.md                           # Main skill instructions and command handlers
        └── references/
            └── cv.md                          # Embedded candidate CV (Single Source of Truth)
```
