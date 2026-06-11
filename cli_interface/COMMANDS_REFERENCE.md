# Slash Commands Reference

Quick reference for all available therapeutic commands.

## Core Therapy Commands

### `/therapy-session`
**Full therapeutic conversation session**

**When to use:**
- Daily emotional processing and support
- Working through difficult emotions or situations
- Diary-style journaling in conversation format
- Deep exploration of patterns and insights
- When you need to talk things through

**What happens:**
1. Warm greeting and connection
2. Mood, energy, and sleep check (1-10 scale)
3. Brief body scan for grounding
4. 3 probing questions based on your patterns
5. Open conversation following your lead
6. Research-backed insights and clinical frameworks
7. Symptom identification and naming
8. Insights summary and gentle homework
9. Session saved to `sessions/YYYY-MM/`

**Time:** 20-45 minutes

**Output:**
- In-chat therapeutic conversation
- Session notes saved automatically
- Daily diary entry in conversational format

---

### `/daily-check`
**Quick 5-minute mental health check-in**

**When to use:**
- Morning or evening wellness check
- Days when you don't need a full session
- Tracking mood and stress trends
- Getting one quick coping strategy

**What happens:**
1. Quick ratings (mood, energy, sleep, stress: 1-10)
2. One-word descriptor for the day
3. Brief symptom identification if needed
4. One micro-intervention (under 2 minutes)
5. Saved to `sessions/YYYY-MM/daily_checks.json`

**Time:** 5 minutes

**Output:**
- Daily metrics tracked
- One actionable coping skill
- Brief validation and support

---

## Roadmap & Progress Commands

### `/create-roadmap`
**Build your personalized 3-6 month developmental roadmap**

**When to use:**
- First time setup (after completing profile)
- Every 3-6 months to create new roadmap
- When ready to set intentional goals
- Major life transitions

**What happens:**
1. Vision exploration (6-month future)
2. Values clarification
3. Goal setting across life areas:
   - Emotional wellbeing
   - Identity development
   - Relationships
   - Life structure
   - Meaning and purpose
4. Milestone planning (monthly)
5. Obstacle and support identification
6. Roadmap saved to `roadmaps/current_roadmap.json`

**Time:** 20-30 minutes

**Output:**
- Comprehensive developmental roadmap
- 3-5 major goals with milestones
- Action steps and progress tracking

---

### `/view-roadmap`
**Review and update your current roadmap**

**When to use:**
- Monthly progress check-ins
- When you want to see your goals
- Celebrating milestones achieved
- Adjusting goals as you evolve
- Feeling lost or unfocused

**What happens:**
1. Display current roadmap
2. Review progress on each goal
3. Celebrate achievements
4. Identify what needs adjustment
5. Update roadmap based on feedback

**Time:** 10-15 minutes

**Output:**
- Visual progress overview
- Milestone celebration
- Updated roadmap (if changes made)

---

## Profile & Context Commands

### `/update-profile`
**Update your psychological profile**

**When to use:**
- New personality assessment results
- Life circumstances change
- Therapy goals evolve
- Coping strategies update
- Support system changes
- New stressors or triggers

**What happens:**
1. Review current profile
2. Guided update conversation
3. Update specific sections
4. Save changes with timestamp
5. Confirm updates

**Time:** 10 minutes

**Output:**
- Updated `profile/personality_assessment.json`
- Timestamp of changes
- Confirmation of what changed

---

### `/load-diary-context`
**One-time load of historical diary entries**

**When to use:**
- First time setup (if you have historical diaries)
- When you want to add historical context
- After collecting diary files to import

**What happens:**
1. Locate diary files in `diary_context/historical/`
2. Extract and process each entry:
   - Emotional patterns
   - Life events and transitions
   - Relationship dynamics
   - Coping mechanisms
   - Values and goals
   - Persistent themes
3. Synthesize narrative understanding
4. Save to `diary_context/diary_context_summary.json`
5. Confirm understanding with you

**Time:** 15-30 minutes (depending on number of entries)

**Output:**
- Comprehensive context summary
- Deep understanding of your journey
- Patterns and themes identified
- Enhanced personalization in all future sessions

**Note:** This is typically done ONCE at setup. After that, daily sessions create ongoing diary context automatically.

---

## Advanced Usage

### Combining Commands

**Recommended flow for new users:**
```
1. Fill out profile/personality_assessment.json
2. /load-diary-context (if you have historical diaries)
3. /create-roadmap
4. /therapy-session (regular use)
5. /daily-check (quick check-in days)
6. /view-roadmap (monthly)
```

**Weekly routine example:**
- Monday-Friday: `/therapy-session` or `/daily-check`
- Saturday: `/view-roadmap` (weekly mini-review)
- Sunday: Longer `/therapy-session` for weekly reflection

**Monthly routine:**
- Week 1: `/view-roadmap` (formal monthly review)
- Week 2-4: Regular sessions
- Last day: `/update-profile` if anything changed

---

## Command Outputs

### What Gets Saved Where

| Command | Output File | Purpose |
|---------|------------|---------|
| `/therapy-session` | `sessions/YYYY-MM/session_YYYY-MM-DD.json` | Full session record |
| `/daily-check` | `sessions/YYYY-MM/daily_checks.json` | Daily metrics |
| `/create-roadmap` | `roadmaps/current_roadmap.json` | Developmental plan |
| `/view-roadmap` | Updates `current_roadmap.json` | Progress tracking |
| `/update-profile` | Updates `profile/personality_assessment.json` | Profile changes |
| `/load-diary-context` | `diary_context/diary_context_summary.json` | Historical context |

### Session Notes Structure

Each therapy session saves:
```json
{
  "date": "YYYY-MM-DD",
  "session_number": X,
  "mood_metrics": {
    "mood_rating": X,
    "energy_level": X,
    "sleep_quality": X,
    "stress_level": X
  },
  "main_themes": ["theme 1", "theme 2"],
  "symptoms_identified": ["symptom 1"],
  "clinical_observations": {},
  "interventions_used": ["CBT", "Self-compassion"],
  "research_shared": [
    "Citation 1 from search"
  ],
  "homework_assigned": "Gentle suggestion",
  "progress_indicators": ["positive sign 1"],
  "concerns_flagged": ["if any"],
  "next_session_focus": "What to explore next"
}
```

---

## Customizing Commands

All commands are stored as markdown files in `.claude/commands/`

**To customize:**
1. Open the command file (e.g., `.claude/commands/therapy-session.md`)
2. Edit Dr. Chen's instructions
3. Modify session structure
4. Adjust communication style
5. Save changes

**Examples of customizations:**
- Change therapist name or persona
- Adjust session length
- Modify probing questions
- Change research citation frequency
- Adjust warmth or directness level

---

## Tips for Effective Use

### For `/therapy-session`
- **Be present**: Give yourself uninterrupted time
- **Be honest**: The AI doesn't judge
- **Ask questions**: Request research, clarification, deeper exploration
- **Follow prompts**: The probing questions are designed to go deeper
- **Take your time**: This is your space

### For `/daily-check`
- **Use consistently**: Daily tracking reveals patterns
- **Be accurate**: Honest ratings help identify trends
- **Try the micro-intervention**: Small practices compound
- **Notice patterns**: Review your `daily_checks.json` periodically

### For `/view-roadmap`
- **Monthly minimum**: Regular reviews maintain momentum
- **Celebrate small wins**: Progress is progress
- **Adjust freely**: Goals should evolve as you do
- **Be kind to yourself**: Missing milestones doesn't mean failure

### For `/update-profile`
- **Update after major changes**: Keeps therapy relevant
- **Update after new insights**: Your self-understanding grows
- **Don't over-update**: Monthly or when significant changes occur

---

## Getting Help During Sessions

**During any session, you can:**
- Ask for research: "What does research say about this?"
- Request clinical terms: "What is this pattern called?"
- Ask for interventions: "What can I do about this?"
- Request gentler/more direct approach: "Can you be more direct?"
- Pause: "I need a moment"
- Redirect: "I want to talk about something else"

**Dr. Chen will:**
- Follow your lead
- Respect your pace
- Provide evidence when helpful
- Name patterns and symptoms
- Offer coping strategies
- Maintain warm professionalism

---

## Troubleshooting

**"Command not found"**
- Ensure you're in the correct directory
- Check `.claude/commands/` folder exists
- Verify the command file is there

**"Dr. Chen seems generic, not personalized"**
- Complete `profile/personality_assessment.json`
- Run `/load-diary-context` if you have historical diaries
- Have 2-3 sessions to build context

**"No research citations appearing"**
- Research is used when relevant, not every session
- Explicitly ask: "What does research say?"
- Check your internet connection (needed for WebSearch)

**"Sessions feel too short/long"**
- Adjust your conversation depth
- Use `/daily-check` for quick check-ins
- Use `/therapy-session` for deeper work

**"I want to change the therapist's style"**
- Edit `profile/preferences.json` → `therapist_persona` → `style`
- Or edit `.claude/commands/therapy-session.md` directly

---

## Quick Reference Table

| Need | Command | Time |
|------|---------|------|
| Daily emotional support | `/therapy-session` | 20-45 min |
| Quick check-in | `/daily-check` | 5 min |
| Set goals | `/create-roadmap` | 30 min |
| See progress | `/view-roadmap` | 10 min |
| Update info | `/update-profile` | 10 min |
| Add diaries | `/load-diary-context` | 15-30 min |

---

**Your therapeutic journey is in your hands. Use these tools in whatever way serves your healing and growth best.**
