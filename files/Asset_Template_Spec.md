# Vertical Asset Template — Build Spec & Production SOP

Build this once. Every client asset after that is a fill-in, which is what turns 16 assets/month into ~8 hours instead of 25.

---

## 1. Sequence settings

| Setting | Value |
|---|---|
| Resolution | 1080 × 1920 (9:16) |
| Frame rate | Match source (23.976 / 24 / 29.97 — never mix within one asset) |
| Color space | Rec. 709 |
| Audio | 48 kHz stereo |

---

## 2. Safe zones

Platform UI covers the edges of the frame. Anything important outside this band gets hidden behind buttons and captions.

```
      0 ┌─────────────────────────┐
        │   ✗  platform header    │
    350 ├─────────────────────────┤
        │                         │
        │      SAFE ZONE          │
        │   all faces, all text   │
        │      lives here         │
        │                         │
   1450 ├─────────────────────────┤
        │  ✗ caption bar, CTA,    │
        │    audio ticker         │
   1920 └─────────────────────────┘
        ✗ right 200px — action buttons (TikTok/Reels)
```

- **Vertical safe band:** y = 350 → 1450
- **Right margin:** keep text and faces out of the right 200 px
- **Subject framing:** eyes at roughly y = 700–850

---

## 3. Caption styling

Burned-in captions are non-negotiable — the large majority of social video is watched muted, and captions are the single biggest driver of completion rate.

| Property | Value |
|---|---|
| Typeface | Heavy sans — Inter Black, Montserrat ExtraBold, or client brand font |
| Size | 64–76 px |
| Case | Sentence case (ALL CAPS reads as shouting and hurts legibility at length) |
| Color | White, #FFFFFF |
| Contrast | 5 px dark stroke **or** 60% black rounded box — pick one, keep it consistent |
| Position | y ≈ 1150–1350 |
| Line rules | 2–4 words per line, maximum 2 lines on screen |
| Timing | Word-level or phrase-level sync — never a full paragraph at once |

---

## 4. Structure of every asset

| Time | What happens |
|---|---|
| 0.0 – 1.5s | **The hook.** Strongest sentence in the clip, plus motion. No logo, no title card. |
| 1.5 – 5s | Establish who's speaking — lower third, name + role, out by 5s |
| 5s – end | The substance |
| Final 1.5s | Client logo + handle. Small, corner, non-blocking. |

**Total length: 30–60 seconds.** Under 30 reads as thin; over 60 collapses completion rate.

The most common failure is opening with a branded intro card. Every second before the hook costs viewers. Brand at the end, never the front.

---

## 5. Export preset

| Setting | Value |
|---|---|
| Format | H.264 / MP4 |
| Bitrate | VBR 2-pass, target 12 Mbps, max 16 Mbps |
| Audio | AAC, 320 kbps, 48 kHz |
| Loudness | Normalize to **−14 LUFS integrated** (social standard) |
| Peak ceiling | −1.0 dBTP |

Save as a named preset — `9x16_Social_Master` — so export is one click.

---

## 6. File naming

```
CLIENT_YYYYMMDD_SOURCE_TOPIC_v01_9x16.mp4
```

Example: `PFF_20261002_DirectorsPanel_FundingIndie_v01_9x16.mp4`

Consistent naming is what makes a shared folder navigable to a client. It also makes you look like a company rather than a student, which is worth more than it sounds.

---

## 7. The five-stage pipeline

Straight from §2.2 of your blueprint. Build it now at one client so it holds at three.

| Stage | What happens | Tool | Time |
|---|---|---|---|
| **1. Intake** | Client drops raw footage in a shared folder | Google Drive or Frame.io | client-side |
| **2. Transcribe** | Auto-transcribe the full session | FCP's Transcribe to Captions, or MacWhisper / Descript | 10 min |
| **3. Select** | Read the transcript, mark 6–10 moments. **Do not scrub video to find clips** — read text. This is the single biggest time save in the whole workflow. | Transcript | 25 min |
| **4. Assemble** | Drop selects into the template, auto-caption, correct names and jargon, brand out | Final Cut Pro | 20 min/asset |
| **5. Review → publish** | Client reviews in one batch, you schedule | Frame.io + scheduler | 45 min/batch |

**Rule: one review round, batched.** Unlimited revisions is what destroys margin on retainer work. Put it in writing: one consolidated round of notes per batch.

---

## 8. Monthly deliverable mix (16 assets)

For a festival or production-company client:

| Type | Count | Source |
|---|---|---|
| Talking-head pull-quotes | 8 | Panels, Q&As, filmmaker interviews |
| B-roll / atmosphere montage | 3 | Venue, audience, red carpet |
| Announcement / promo | 2 | Programming news, ticket pushes |
| Sponsor-facing recap | 2 | Sponsor-attributed moments |
| Flex | 1 | Whatever they ask for |

The sponsor-facing pieces matter more than their count suggests. Festivals owe sponsors visibility, and proof of delivered impressions is what renews sponsorship money. Being the person who makes that easy is how you become hard to cut.

---

## 9. Build checklist

Built in **Final Cut Pro** — you own it outright, commercial use is permitted, and it doesn't lapse between semesters. See the licensing section of the countdown plan.

- [ ] Custom 1080×1920 project preset saved
- [ ] Safe-zone guide overlay saved (generator or still on a top layer)
- [ ] Caption style saved as a Title template / Compound Clip
- [ ] Lower-third template built (name + role, 3.5s animation)
- [ ] End card built (logo + handle, 1.5s)
- [ ] Export preset `9x16_Social_Master` saved
- [ ] Loudness normalization step confirmed
- [ ] Naming convention written into the client folder README
- [ ] One full spec asset cut end-to-end and timed

That last item is the real test. Cut one complete asset and time yourself. If it's over 35 minutes, the template isn't finished — find the step that's still manual and template it.
