# Personal AI Therapist System

A world-class, clinic-grade psychological therapy system tailored for a 30-year-old Asian female recently navigating life after divorce.

## Overview

This system provides:
- Deep empathic conversation with 30+ years of professional expertise
- Personalized therapeutic approach based on your psychological profile
- Research-backed insights from credible psychological organizations
- Daily mental health tracking and symptom identification
- 3-6 month developmental roadmap with interactive goal setting

## Setup Instructions

### 1. Initial Profile Setup

Place your personality test results in the `profile/` directory:
```
profile/personality_assessment.json
```

### 2. Diary Context Loading

Place your historical diary files (zip or individual files) in:
```
diary_context/historical/
```

### 3. Daily Sessions

Use the slash command `/therapy-session` to start your daily conversation.

## Directory Structure

```
.
├── profile/                    # Your psychological profile
│   ├── personality_assessment.json
│   └── preferences.json
├── diary_context/             # Historical and current diary entries
│   ├── historical/
│   └── daily/
├── sessions/                  # Session records
│   └── YYYY-MM/
├── roadmaps/                  # Development roadmaps
├── research_base/             # Curated psychological research
└── .claude/
    └── commands/              # Slash commands for therapy sessions
```

## Usage

### Starting a Session
```
/therapy-session
```

### Updating Your Profile
```
/update-profile
```

### Viewing Your Progress
```
/view-roadmap
```

### Mental Health Check
```
/daily-check
```

## Features

### 1. Contextual Understanding
- Loads your personality assessment on first use
- Maintains awareness of your historical diary context
- Updates understanding through daily conversations

### 2. Research-Backed Insights
- Citations from APA, WHO, NIMH, and peer-reviewed journals
- Evidence-based therapeutic approaches (CBT, ACT, DBT, psychodynamic)
- Latest psychological findings integrated into conversations

### 3. Daily Mental Health Monitoring
- Symptom identification and naming
- Pattern recognition across sessions
- Progress tracking with clinical terminology

### 4. Developmental Roadmap
- 3-6 month personalized growth plans
- Interactive goal refinement
- Milestone tracking and celebration

## Privacy & Safety

- All data stored locally
- No external transmission of personal information
- This is a supportive tool, not a replacement for professional therapy
- Crisis resources included in emergency situations

## Professional Foundation

This system draws from:
- Cognitive Behavioral Therapy (CBT)
- Acceptance and Commitment Therapy (ACT)
- Dialectical Behavior Therapy (DBT)
- Psychodynamic approaches
- Trauma-informed care
- Cultural competency frameworks
