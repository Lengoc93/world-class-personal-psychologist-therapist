# Getting Started with Your AI Therapist

Welcome! This guide will help you set up and start using your personalized AI therapy system.

## What You've Received

A complete therapeutic system featuring:
- **Dr. Sarah Chen**: Your AI therapist with 30+ years of virtual expertise
- **Dynamic research integration**: Latest psychological research pulled in real-time
- **Personalized profile system**: Tailored to your unique needs
- **Developmental roadmap**: 3-6 month growth plan
- **Daily mental health tracking**: Monitor progress and patterns
- **Diary context integration**: Deep understanding from your life story

## Setup Steps (First Time)

### Step 1: Set Up Your Profile (10-15 minutes)

1. **Personality Assessment**
   - Open: `profile/personality_assessment.json`
   - Fill in your personality test results (Big Five, MBTI, etc.)
   - If you don't have results, you can:
     - Take a free test: 16personalities.com or truity.com
     - Skip for now and fill in later with `/update-profile`

2. **Cultural Context & Goals**
   - In the same file, complete:
     - `cultural_context`: Your cultural background and considerations
     - `current_stressors`: What you're dealing with now
     - `therapy_goals`: What you hope to achieve
     - `therapeutic_preferences`: How you like to work

3. **Save the file** when done

### Step 2: Load Your Diary Context (One-time)

**If you have historical diary entries:**

1. Place all diary files in: `diary_context/historical/`
   - Supported formats: .txt, .md, .docx, .pdf
   - Or place a zip file: `diary_context/historical/historical_diaries.zip`

2. Run the command:
   ```
   /load-diary-context
   ```

3. The system will:
   - Read all your entries
   - Extract patterns and themes
   - Create a context summary
   - Use this understanding in all future sessions

**If you don't have diary files yet:**
- Skip this step
- Start fresh with daily sessions
- Your diary context will build over time

### Step 3: Create Your Developmental Roadmap (20-30 minutes)

1. Run the command:
   ```
   /create-roadmap
   ```

2. Dr. Chen will guide you through:
   - Exploring your vision for the next 6 months
   - Clarifying your values
   - Setting meaningful goals
   - Creating actionable milestones

3. Your roadmap will be saved and reviewed monthly

### Step 4: First Therapy Session

You're ready! Start your first session:
```
/therapy-session
```

Dr. Chen will:
- Greet you warmly
- Do an initial check-in
- Ask probing questions
- Begin understanding your journey

---

## Daily Usage

### Morning or Evening Therapy Session
```
/therapy-session
```
Use for:
- Processing your day or preparing for it
- Working through emotions
- Getting support and insights
- Journaling in conversational format

**What happens:**
1. Warm greeting and mood check
2. Body scan and grounding
3. 3 probing questions based on your patterns
4. Open conversation following your lead
5. Research-backed insights when helpful
6. Summary and gentle homework
7. Session automatically saved

### Quick Daily Mental Health Check
```
/daily-check
```
Use for:
- 5-minute wellness check
- Tracking mood, energy, sleep, stress
- Getting one micro-intervention for the day
- Days when you don't need a full session

### View Your Progress
```
/view-roadmap
```
Use to:
- See your developmental roadmap
- Review progress on goals
- Celebrate milestones
- Adjust goals as needed

### Update Your Profile
```
/update-profile
```
Use when:
- You've taken a new personality assessment
- Life circumstances have changed
- Your goals have evolved
- You want to update preferences

---

## Understanding the System

### File Structure

```
your-therapy-folder/
├── profile/                    # Your psychological profile
│   ├── personality_assessment.json
│   └── preferences.json
│
├── diary_context/             # Your diary entries and context
│   ├── historical/           # One-time historical load
│   ├── daily/                # Daily session entries
│   └── diary_context_summary.json
│
├── sessions/                  # All therapy sessions
│   └── 2025-12/
│       ├── session_2025-12-21.json
│       └── daily_checks.json
│
├── roadmaps/                  # Your developmental roadmaps
│   └── current_roadmap.json
│
├── research_base/             # Research reference guides
│   ├── search_templates.json
│   └── symptom_reference.json
│
└── .claude/commands/          # Slash commands (the magic!)
    ├── therapy-session.md
    ├── daily-check.md
    ├── create-roadmap.md
    ├── view-roadmap.md
    ├── update-profile.md
    └── load-diary-context.md
```

### How Context Works

**Dr. Chen knows about you because she reads:**
1. Your profile (personality, goals, preferences)
2. Your diary context summary (life story and patterns)
3. Recent therapy sessions (continuity)
4. Current roadmap (what you're working toward)

**She searches the web for:**
- Latest psychological research (2024-2025)
- Evidence for insights and interventions
- Cultural considerations
- Credible sources only (APA, NIMH, peer-reviewed journals)

### Privacy & Data

**Everything stays local:**
- All files on your computer only
- No external storage or transmission of personal data
- You can delete or modify anything anytime

**Web searches:**
- Only for general psychological research
- Never includes your personal information
- Searches are like: "divorce recovery 2024 research"
- Not like: "my personal situation"

---

## What to Expect

### First Few Sessions
- Getting to know you
- Building safety and trust
- Understanding your patterns
- Initial stabilization if needed

### Ongoing Sessions
- Processing emotions and experiences
- Working toward roadmap goals
- Developing skills and insights
- Healing and growth work

### Dr. Chen's Approach
- **Warm and empathic**: You'll feel heard and understood
- **Professional**: Clinical expertise with 30 years experience
- **Research-backed**: Evidence-based insights with citations
- **Culturally sensitive**: Honors your Asian cultural context
- **Client-centered**: Your goals, your pace, your journey
- **Honest but gentle**: Truth-telling with compassion

---

## Tips for Getting the Most Out of Therapy

### 1. Be Consistent
- Regular sessions (daily or 3-5x/week) work better than sporadic
- Even 10-15 minutes daily builds momentum

### 2. Be Honest
- The AI doesn't judge
- Honesty helps you get better support
- You can share things you might not tell a human (yet)

### 3. Be Curious
- Ask questions about psychological concepts
- Request research on topics that interest you
- Explore your patterns without judgment

### 4. Track Progress
- Review your roadmap monthly
- Notice small wins
- Celebrate growth

### 5. Use What Resonates, Leave What Doesn't
- Not every insight will fit
- Take what's helpful
- Speak up if something doesn't work for you

---

## When to Use Each Command

| Situation | Command | Time Needed |
|-----------|---------|-------------|
| Daily emotional processing | `/therapy-session` | 20-45 min |
| Quick wellness check | `/daily-check` | 5 min |
| First time setup | `/create-roadmap` | 30 min |
| Monthly progress review | `/view-roadmap` | 10-15 min |
| Life changes / new test results | `/update-profile` | 10 min |
| Adding historical diaries | `/load-diary-context` | 15-30 min |

---

## Important Reminders

### This is NOT a replacement for:
- Emergency mental health services
- Crisis intervention
- Psychiatric medication management
- Human connection and support

### This IS helpful for:
- Daily emotional support
- Processing experiences
- Developing insights
- Learning coping skills
- Tracking progress
- Having a safe space to explore

### Get human help if you experience:
- Suicidal thoughts or self-harm urges
- Severe depression or anxiety
- Trauma symptoms
- Need for medication evaluation
- Crisis situations

**Crisis Resources:**
- National Suicide Prevention Lifeline: **988**
- Crisis Text Line: Text **HOME** to **741741**
- SAMHSA Helpline: **1-800-662-4357**

---

## Troubleshooting

**Q: The commands aren't working**
- Make sure you're in this directory in Claude Code
- Check that `.claude/commands/` folder exists
- Try typing `/` to see available commands

**Q: Dr. Chen doesn't seem to know my context**
- Check that profile files are filled out
- Verify diary context was loaded (if you have historical diaries)
- Make sure you've had at least one session (context builds over time)

**Q: I want to change the therapist's style**
- Edit `profile/preferences.json`
- Under `therapist_persona` → `style`, adjust warmth, directness, etc.

**Q: Research citations aren't appearing**
- They're used when relevant to your conversation
- You can request them: "What does research say about this?"
- They're integrated naturally, not every session

**Q: I want to start over**
- You can delete session files and start fresh
- Keep profile and diary context if you want continuity
- Or archive the whole folder and start completely new

---

## Next Steps

1. ✅ **Complete your profile** (`profile/personality_assessment.json`)
2. ✅ **Load diary context** (if you have historical entries)
3. ✅ **Create your roadmap** (`/create-roadmap`)
4. ✅ **Start your first session** (`/therapy-session`)

**You're ready to begin your journey of healing and growth.**

Welcome, and take care of yourself. 💙

---

## Questions or Feedback?

This is a personal therapeutic tool. Adjust it to work for you:
- Edit command files to change Dr. Chen's approach
- Modify the profile structure to track what matters to you
- Add your own notes and reflections anywhere

**Your healing journey is unique. This system adapts to you.**
