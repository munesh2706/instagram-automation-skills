---
name: insta-video-production
description: Use this skill to create polished Instagram videos from scripts, voiceovers, and assets. Handles video editing, syncing voiceover to visuals, adding text overlays, transitions, captions, and formatting for 9:16 vertical aspect ratio. Supports free tools (FFmpeg, CapCut, DaVinci Resolve) and premium software. Use AFTER voiceover generation, BEFORE caption/hashtag writing.
---

# Instagram Video Production

## Purpose
Create videos that:
- **SYNC VOICEOVER TO VISUALS** (audio-visual alignment)
- **9:16 VERTICAL FORMAT** (optimized for Instagram)
- **ENGAGING VISUALS** (keeps viewers watching)
- **TEXT OVERLAYS** (reinforce key points)
- **ACCESSIBILITY CAPTIONS** (auto-captions + CC)
- **SMOOTH TRANSITIONS** (professional feel, not jarring)
- **POLISHED AUDIO** (clean voiceover + background music)

## Video Editor Options

| Tool | Cost | Ease | Quality | Best For |
|------|------|------|---------|----------|
| **CapCut** | Free | Very Easy | Good | Beginners, simple editing |
| **DaVinci Resolve** | Free (+ paid) | Medium | Excellent | Professional results |
| **Adobe Premiere** | $20/mo | Medium | Excellent | Advanced, premium |
| **Final Cut Pro** | $300 one-time | Medium | Excellent | Mac-focused creators |
| **FFmpeg** | Free | Hard (CLI) | Excellent | Batch processing, automation |

**Recommendation for Instagram**: **DaVinci Resolve** (free, professional quality)

## Pre-Production Checklist

### Assets You Need:
- [ ] Voiceover MP3 (from previous step)
- [ ] Video footage (30-60 seconds of B-roll)
- [ ] Images (if using stock photos instead of video)
- [ ] Text/graphics (any titles, stats, overlays)
- [ ] Background music (royalty-free, Instagram-friendly)
- [ ] Script (for timing reference)

### Where to Get Free Assets:

**Stock Video & Images**:
- Pexels (pexels.com) - Free, no attribution
- Pixabay (pixabay.com) - Free, no attribution
- Unsplash (unsplash.com) - Free, no attribution
- Coverr (coverr.co) - Free short videos

**Royalty-Free Music**:
- Epidemic Sound (epidemic.com) - $9/mo
- Artlist (artlist.io) - $10/mo
- Incompetech (incompetech.com) - Free
- YouTube Audio Library (youtube.com/audio) - Free

**Free Font Libraries**:
- Google Fonts (fonts.google.com)
- DaFont (dafont.com)

## Video Production Workflow

### Step 1: Gather & Organize Assets

Create folder structure:
```
Project/
├── footage/
│   ├── b-roll-1.mp4
│   ├── b-roll-2.mp4
│   └── b-roll-3.mp4
├── voiceover/
│   └── topic_voiceover.mp3
├── music/
│   └── background_music.mp3
├── graphics/
│   ├── stat-1.png
│   ├── stat-2.png
│   └── title.png
└── script.txt
```

### Step 2: Import Assets into Editor

**Using DaVinci Resolve**:
1. Create new project (9:16 aspect ratio, 1080×1920 pixels)
2. Import media: File → Import → Select all assets
3. Drag to timeline:
   - Video track 1: B-roll footage
   - Audio track 1: Voiceover
   - Audio track 2: Background music
   - Text track: Titles & overlays

### Step 3: Sync Voiceover to Visuals

**Basic sync process**:
1. Place voiceover on audio track
2. Trim/arrange B-roll to match voiceover length
3. Listen and watch together
4. Adjust B-roll cuts to match voiceover pacing
5. Add visual interest: cut to new footage every 3-5 seconds

**Example timeline**:
```
[0-5s] Hook voiceover → Cut to animated title
[5-15s] Problem setup → Show relatable scenario footage
[15-25s] Example story → Show person/situation visuals
[25-35s] Solution explanation → Show step-by-step graphics
[35-45s] Example results → Show before/after visuals
[45-55s] Big promise → Show aspirational footage
[55-60s] CTA → Show profile/bio link graphic
```

### Step 4: Add Text Overlays

**Key moments to add text**:
- Hook (0-3s): Large text, center bottom
- Key numbers (during examples): Highlight in bright color
- Solution steps: One text per step
- Results/stats: Large numbers, clear font
- CTA (55-60s): "Follow" or "Link in bio"

**Text overlay specs**:
- Font: Clean, sans-serif (Montserrat, Raleway, Poppins)
- Size: Large enough to read on phone (24pt minimum)
- Color: High contrast (white text on dark background, or vice versa)
- Duration: 3-5 seconds per overlay
- Animation: Fade in/out (0.3 seconds), not harsh

**Example text in DaVinci**:
```
Text: "Your bank account is bleeding $1000/month"
Font: Montserrat Bold, 48pt, White
Position: Center, bottom 1/3 of frame
Duration: 3 seconds
Animation: Fade in (0.3s) + Fade out (0.3s)
```

### Step 5: Add Transitions

**Best transitions for Instagram**:
- **Cut** (no transition): 80% of cuts (default)
- **Fade** (0.3s): Between major sections
- **Dissolve** (0.2s): Between related visuals
- **Zoom in/out** (0.2s): For emphasis on key moments

**Avoid**:
- ❌ Spinning/fancy transitions (distracting)
- ❌ Long transitions (>0.5 seconds, slows pacing)
- ❌ Multiple transition styles (looks unprofessional)

**Rule**: 90% cuts, 10% fades/dissolves

### Step 6: Audio Mixing

**Voiceover volume**: -3 to 0 dB (should be primary)
**Background music volume**: -18 to -12 dB (quiet, doesn't compete)
**Level**: Monitor levels to avoid clipping

**Audio mixing steps**:
1. Import voiceover on audio track 1
2. Import background music on audio track 2
3. Drag background music volume slider down to -15 dB
4. Listen to both together
5. Make sure voiceover is clear and dominant
6. Add fade-out to background music at end (2 seconds)

### Step 7: Add Captions (Auto-Captions)

**DaVinci Resolve method**:
1. Right-click voiceover clip
2. Select "Subtitle" → "Add Subtitles"
3. Choose "Transcribe" → "Speech-to-Text"
4. Review transcript (correct any errors)
5. Generate captions
6. Style captions: white text, black background, large font

**Alternative: YouTube Auto-Captions**
1. Upload unlisted to YouTube
2. Wait 24 hours for auto-captions
3. Download caption file
4. Import to video editor

**Caption specs for Instagram**:
- Font: Sans-serif, 20-24pt
- Color: White text, black background with opacity
- Position: Bottom 1/3 of frame (doesn't block action)
- Timing: Match voiceover exactly
- Style: Conversational tone (not formal, not slang)

### Step 8: Final Export Settings

**For Instagram**:
- **Resolution**: 1080 × 1920 pixels (vertical 9:16)
- **Frame rate**: 30 fps (standard for Instagram)
- **Codec**: H.264 (MP4 format, compatible)
- **Bitrate**: 8-12 Mbps (high quality)
- **Audio**: 128 kbps, stereo

**DaVinci export settings**:
```
Format: MP4
Resolution: 1080 × 1920
Frame Rate: 30 fps
Codec: H.264
Quality: High
Color Space: Rec.709
Metadata: Include (for captions)
```

**File naming**:
`[topic]_[date]_[version].mp4`
Example: `budgeting-basics_2026-10-26_v1.mp4`

## Using CapCut (Easy Alternative)

**CapCut workflow** (phone/desktop):
1. Open CapCut, create new project
2. Import voiceover
3. Import B-roll footage
4. Trim footage to match voiceover length
5. Add transitions (auto-add or manual)
6. Add text overlays (tap "Text" button)
7. Add background music
8. Export (select vertical 9:16 format)

**CapCut advantages**: Easiest for beginners, built-in auto-captions, fast

## Using FFmpeg (Automation)

For batch processing multiple videos:

```bash
ffmpeg -i video.mp4 -i voiceover.mp3 \
  -vf "scale=1080:1920,setsar=1" \
  -c:v libx264 -c:a aac \
  -shortest output.mp4
```

**Explanation**:
- `-i video.mp4`: Input video file
- `-i voiceover.mp3`: Input audio file
- `-vf "scale=1080:1920"`: Resize to 9:16
- `-c:v libx264`: Video codec (H.264)
- `-c:a aac`: Audio codec
- `-shortest`: Cut to shortest input length
- `output.mp4`: Output file

## Visual Style for Instagram

### Color Grading:
- **Bright & energetic**: Increase saturation +15%, brightness +5%
- **Calm & educational**: Decrease saturation -10%, increase contrast
- **Professional**: Neutral color grade, slight warm filter

### Typography:
- **Headline**: Bold, large (Montserrat Bold, 48-60pt)
- **Body text**: Regular weight, medium (Raleway Regular, 24-32pt)
- **Accent**: One accent color (brand color or bright color for emphasis)

### B-Roll Pacing:
- Change footage every 3-5 seconds (keeps viewers engaged)
- Show related visuals (don't use random B-roll)
- Use smooth zooms/pans (not jarring cuts)

## Common Video Production Mistakes

| Mistake | Fix |
|---------|-----|
| Voiceover doesn't match length | Trim voiceover or add more B-roll |
| Text overlays hard to read | Use larger font, higher contrast |
| B-roll doesn't match topic | Use relevant visuals (not random) |
| Too many transitions | Use 90% cuts, 10% fades |
| Audio levels inconsistent | Normalize voiceover + background music |
| Captions out of sync | Fix in editor, review before export |
| Wrong aspect ratio | Make sure project is 9:16 (1080×1920) |
| Video file too large | Lower bitrate to 8-10 Mbps |

## Video Production Checklist

- [ ] All assets imported into editor
- [ ] Voiceover synced to B-roll (watched full video)
- [ ] Text overlays added at key moments
- [ ] Captions auto-generated or manually added
- [ ] Background music added and mixed correctly
- [ ] Transitions minimal (cuts 90%, fades 10%)
- [ ] Color grading applied consistently
- [ ] Final review: Watch full video for quality
- [ ] Audio levels checked (no clipping)
- [ ] Export settings correct (1080×1920, H.264, 8-12 Mbps)
- [ ] File size reasonable (<200 MB for 60-second video)
- [ ] File naming convention applied
- [ ] Backup saved to cloud storage

## File Storage & Backup

Save in this structure:
```
Videos/
├── Raw/
│   ├── [topic]_voiceover.mp3
│   ├── [topic]_broll_[date].mp4
│   └── [topic]_music.mp3
├── Projects/
│   └── [topic]_project_davinci.ddb (editor file)
├── Final/
│   └── [topic]_final_[date].mp4
└── Backup/
    └── [monthly backup of everything]
```

## Time-Saving Tips

### Tip 1: Create Templates
- Build a "title template" in your editor
- Build a "text overlay template"
- Reuse for every video (saves 30 minutes)

### Tip 2: Batch B-Roll
- Shoot 30-60 seconds of related B-roll
- Use it across 5-10 videos
- Prevents repetition while saving time

### Tip 3: Music Track Library
- Create 5 go-to background music tracks
- Rotate them across videos
- Consistent audio branding

### Tip 4: Shortcut Keys
- Learn keyboard shortcuts in your editor
- Cuts 50% of editing time
- Example: Space = Play/Stop, V = Cut tool
