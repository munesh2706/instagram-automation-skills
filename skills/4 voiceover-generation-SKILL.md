---
name: insta-voiceover-generation
description: Use this skill to generate professional AI voiceovers for Instagram scripts. Supports ElevenLabs, Google Cloud TTS, Azure, Synthesia, and others. Creates natural-sounding voiceovers with customizable tone, speed, accent, and emotion. Handles script timing, multiple voice options, and audio optimization. Use AFTER script writing, BEFORE video production.
---

# Instagram AI Voiceover Generation

## Purpose
Generate voiceovers that:
- **SOUND NATURAL** (not robotic or AI-obvious)
- **MATCH SCRIPT PACING** (sync words to timing)
- **CUSTOMIZE TONE** (conversational, authoritative, emotional)
- **MATCH BRAND VOICE** (consistent across videos)
- **OPTIMIZE AUDIO** (clear, balanced, no background noise)
- **HANDLE TIMING** (exact timing for video sync)

## Supported Voiceover Platforms

| Platform | Quality | Cost | Voice Options | Best For |
|----------|---------|------|----------------|----------|
| **ElevenLabs** | Excellent | $5-99/mo | 29+ voices, custom cloning | Most natural, emotional range |
| **Google Cloud TTS** | Very Good | $4-16 per 1M chars | 100+ voices, multiple languages | Consistent, scalable |
| **Azure (Microsoft)** | Very Good | $4 per 1M chars | 400+ voices, neural voices | Professional, many accents |
| **Synthesia** | Good | $30-150/mo | AI avatars + voiceover combined | Video with avatar included |
| **Descript** | Good | $12-24/mo | Limited voices, local processing | Simple, integrated editing |
| **PlayHT** | Very Good | $10-99/mo | 100+ voices, custom voices | Affordable, high quality |

**Recommendation for Instagram**: **ElevenLabs** (most natural sound, best for content creators)

## Process: Step-by-Step

### Step 1: Prepare the Script
Before generating voiceover:
- [ ] Script is final (no changes after voiceover)
- [ ] Word count matches target length
- [ ] All numbers written out phonetically if unclear
- [ ] Punctuation marks correct (for pauses)
- [ ] No bracketed instructions in final version

**Example script prep**:
```
BEFORE: "That's $750/month = $9000/year just GONE."
AFTER: "That's seven hundred fifty dollars per month, 
which equals nine thousand dollars per year, just gone."
```

### Step 2: Choose Your Voice (ElevenLabs Example)

#### Factors to Consider:

**A. Voice Gender & Age**
- Neutral, Female, Male
- Young adult (20-40), Mature (40-60)
- Decision: Should match your brand identity

**B. Voice Tone**
- Conversational (friendly, relatable)
- Authoritative (confident, expert)
- Energetic (excited, motivational)
- Empathetic (understanding, supportive)
- **For Instagram**: Conversational or Energetic

**C. Accent**
- American, British, Australian, etc.
- **For Instagram**: Depends on target audience

**D. Speed**
- Slow (80 WPM): Formal, deliberate
- Normal (120-150 WPM): Conversational, natural
- Fast (180 WPM): Energetic, urgent
- **For Instagram 60-sec video**: Normal to Fast

**E. Emotional Style** (ElevenLabs specific)
- Calm
- Sad
- Angry
- Surprised
- Happy
- Friendly
- Excited
- **For Instagram**: Friendly or Excited

### Step 3: Voice Selection Recommendation

**For Educational Content**:
- **Voice**: Female, conversational tone, normal-fast speed
- **Emotion**: Friendly + Slightly Excited
- **Accent**: Your audience's accent (if international, American English is default)

**For Motivational Content**:
- **Voice**: Male or Female, energetic tone, fast speed
- **Emotion**: Excited + Happy
- **Accent**: American English or Australian

**For Complex Topics (ELI5)**:
- **Voice**: Female, conversational, slower speed
- **Emotion**: Friendly + Helpful
- **Accent**: Clear, standard

### Step 4: Generate Voiceover

#### Option A: Using ElevenLabs API

**Setup** (if you're a developer):
```bash
pip install elevenlabs

# Set API key
export ELEVEN_API_KEY="sk_..."

# Generate voiceover
elevenlabs \
  --text "Your full script here..." \
  --voice "Rachel" \
  --output "voiceover.mp3" \
  --stability 0.5 \
  --similarity_boost 0.75
```

**Parameters explained**:
- `voice`: "Rachel", "Adam", "Bella", etc. (choose from available)
- `stability`: 0-1 (higher = more consistent, lower = more emotional variation)
- `similarity_boost`: 0-1 (higher = more similar to original voice)
- **Recommended**: stability=0.5, similarity_boost=0.75 (natural + expressive)

#### Option B: Using ElevenLabs Web Interface

1. Go to elevenlabs.io
2. Sign up (free tier: 10k characters/month)
3. Click "Speech Synthesis"
4. Paste your script
5. Choose voice + settings
6. Click "Generate"
7. Download MP3

**Settings**:
- Voice: [Choose your selected voice]
- Stability: 0.50
- Similarity Boost: 0.75
- Style Exaggeration: 0 (leave default)

#### Option C: Using Google Cloud TTS

```bash
gcloud text-to-speech synthesize-speech \
  --text="Your script" \
  --language-code=en-US \
  --name=en-US-Neural2-C \
  --audio-encoding=MP3 \
  --output-file=voiceover.mp3 \
  --pitch=0 \
  --speaking-rate=1.2
```

**Parameters**:
- `language-code`: en-US, en-GB, etc.
- `name`: Neural voice options (sounds most natural)
- `speaking-rate`: 0.25-4.0 (1.0 = normal, 1.2 = 20% faster)
- `pitch`: -20 to 20 semitones (0 = default)

#### Option D: Using Azure

```bash
# Use Azure Cognitive Services SDK
# See Azure documentation for full setup
```

### Step 5: Timing Verification

**Calculate expected audio length**:
```
Script word count ÷ Speaking speed = Duration

Example:
150 words ÷ 2.5 words/sec = 60 seconds ✓
```

**If voiceover is too long**:
- Edit script to remove 20-30 words
- Regenerate voiceover
- Re-sync with video

**If voiceover is too short**:
- Add meaningful content (not filler)
- Slow down speaking rate slightly
- Regenerate

### Step 6: Audio Quality Check

Listen to voiceover for:
- [ ] **Clarity**: Every word is clear, no mumbling
- [ ] **Pacing**: Not too fast or slow, natural flow
- [ ] **Tone**: Matches intended emotion/brand voice
- [ ] **Pronunciation**: All words pronounced correctly
  - If wrong: Add pronunciation guide in script
  - Example: "Quinoa" → "Keen-wah"
- [ ] **No AI artifacts**: No robotic sounds or glitches
- [ ] **Volume consistent**: No sudden loud/quiet sections

**If quality is poor**: Choose different voice or platform

### Step 7: Audio Processing (Optional)

If you have audio editing software (Audacity, Adobe Audition):
- Normalize volume (make consistent)
- Remove background hum (if any)
- Add fade-in at start (0.5 seconds)
- Add fade-out at end (0.5 seconds)
- Export as MP3 (128 kbps minimum)

## Voice Recommendations by Topic

| Topic Type | Recommended Voice | Tone | Speed |
|-----------|------------------|------|-------|
| Personal Finance | Female, warm, clear | Friendly/Supportive | Normal |
| Productivity | Male or Female, energetic | Excited/Motivating | Fast |
| Education | Female, clear | Friendly/Helpful | Normal |
| Wellness | Female, calm | Peaceful/Supportive | Slightly slow |
| Business Tips | Male, authoritative | Confident/Expert | Normal-Fast |
| Lifestyle | Female or Male, casual | Conversational/Friendly | Normal |
| Motivation | Male, powerful | Energetic/Inspiring | Fast |
| Storytelling | Female, emotional | Warm/Engaging | Normal |

## Common Voiceover Issues & Fixes

| Issue | Cause | Fix |
|-------|-------|-----|
| Sounds robotic | Generic voice + generic settings | Try ElevenLabs with emotion settings, increase similarity_boost |
| Too fast to understand | Speaking rate too high | Lower speaking rate to 1.0-1.1 (normal) |
| Awkward pauses | Poor punctuation | Use periods for short pauses, ellipses (...) for longer pauses |
| Words mispronounced | Unclear script | Write phonetically: "Quinoa" → "keen-wah" |
| Volume inconsistent | Platform issue | Use audio editor to normalize |
| Emotional tone flat | Voice choice + settings | Choose voice known for emotion, use higher similarity_boost |
| Audio quality poor | Low-quality platform | Switch to ElevenLabs or Google Cloud TTS |

## Tips for Best Results

### Tip 1: Script Formatting for Voiceover
```
✅ Good:
"Let's say you make $3000 per month. 
Feels like good money, right? 
But by month end... you're broke."

❌ Bad:
"Let's say you make $3000/month. Feels like good money, right? But by month end you're broke."
```

**Why**: Punctuation = pauses. Line breaks = breathing points.

### Tip 2: Avoid Numbers Ambiguity
```
❌ Script: "$750/month = $9000/year"
✅ Script: "Seven hundred fifty dollars per month, 
which is nine thousand dollars per year"
```

**Why**: AI might read "/" weirdly. Write it out.

### Tip 3: Emphasis Markers
Some platforms support emphasis. Use for key words:
```
"Your **bank account** is bleeding money"
→ AI emphasizes "bank account"
```

### Tip 4: Test Multiple Voices
- Generate with 3 different voices
- Pick the one that feels most "you"
- Consistency > Perfection

### Tip 5: Brand Voice Consistency
Once you find a voice you love:
- **Save the settings**: Voice name, stability, similarity_boost, emotion
- **Use same settings** for all future voiceovers
- This creates consistent brand sound across videos

## Cost Breakdown (Monthly Usage)

**Scenario**: 4 videos/week × 60 seconds = 3,840 seconds/month

| Platform | Cost Formula | Monthly Cost |
|----------|-------------|--------------|
| **ElevenLabs** | 385k chars/month (~$9) | $9-30 |
| **Google Cloud** | $4 per 1M chars = 1.5M chars = $6 | $6-12 |
| **Azure** | $4 per 1M chars | $6-12 |
| **Descript** | $12/month (limited) | $12 |
| **PlayHT** | $10/month (starter) | $10-30 |

**Recommendation**: ElevenLabs ($9-30/month) for best quality

## Output Checklist

- [ ] Voiceover MP3 file downloaded
- [ ] Audio length matches script (±2 seconds)
- [ ] Quality checked (clear, natural, correct tone)
- [ ] Naming convention: `[topic]_voiceover_[date].mp3`
- [ ] Backup copy saved (to cloud + local)
- [ ] Voice settings documented (for future consistency)
- [ ] Ready for video editor (next step)

## Integration with Video Editor

**In your video editor** (After Effects, DaVinci Resolve, CapCut):
1. Import video assets (footage, images, graphics)
2. Import voiceover MP3 (on audio track)
3. Trim/align voiceover to match visuals
4. Add text overlays to match voiceover timing
5. Add background music (low volume, under voiceover)
6. Export final video (9:16 vertical format)
