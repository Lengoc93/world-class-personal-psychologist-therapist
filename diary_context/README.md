# Diary Context System

## Purpose
Your historical and daily diary entries provide crucial context for understanding your emotional patterns, growth journey, and unique experiences.

## Setup

### One-Time Historical Load

1. **If you have a zip file of historical diaries:**
   - Place the zip file in `historical/` folder
   - The system will extract and analyze them on first load
   - Name it: `historical_diaries.zip`

2. **If you have individual files:**
   - Place all historical diary files in `historical/` folder
   - Supported formats: .txt, .md, .docx, .pdf
   - Files will be indexed and contextualized

### Daily Diary Sessions

Your daily diary entries will be saved in `daily/YYYY-MM/` folders automatically during therapy sessions.

## What the System Extracts

From your diary entries, the AI therapist will identify:

- **Emotional patterns**: Recurring feelings, triggers, and emotional cycles
- **Relationship dynamics**: How you relate to others and yourself
- **Coping strategies**: What works and what doesn't
- **Values and priorities**: What matters most to you
- **Growth indicators**: Signs of healing and development
- **Stressors**: Persistent or emerging challenges
- **Resilience markers**: Your strengths and resources
- **Narrative themes**: Your life story and meaning-making

## Privacy

- All files remain on your local machine
- No external uploads or cloud storage
- The AI uses this context only within your sessions
- You can delete or modify files anytime

## Example Diary Structure

The AI can work with any diary format, but here's a helpful structure:

```
Date: 2025-12-21

Mood: [How I'm feeling]

Today's Events:
[What happened]

My Thoughts:
[What I'm thinking about]

Emotions:
[What I'm feeling and why]

Gratitudes:
[What I'm thankful for]

Struggles:
[What's difficult right now]

Insights:
[Any realizations or learnings]
```

## First-Time Setup

When you first use the system, it will:
1. Read all historical diary files
2. Create a contextual understanding of your journey
3. Generate an initial narrative summary
4. Save the summary in `diary_context_summary.json`
5. Use this context in all future sessions

This happens ONCE, then the system only reads new daily entries.
