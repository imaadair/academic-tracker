# AI-First Production Workflow

You're right, and the B2B pivot is what changes my answer.

---

## Why I was wrong before

My objection to AI editing was aimed at **film festival clients** — people with visual taste who'd recognize and dislike the AI-clip look. That argument doesn't survive the pivot.

B2B LinkedIn is the opposite environment. The auto-reframe, bouncing-caption aesthetic isn't a tell there — **it's the native format.** Your buyer is a marketing manager who wants volume, consistency, and speed. Nobody is judging your cutting.

---

## The math, which is the real argument

| | Manual in Final Cut | AI-first |
|---|---|---|
| Time per client per month | ~13 hrs | ~5 hrs |
| Clients at 8 hrs/week | 2 | **5–6** |
| Monthly revenue at $1,500 | $3,000 | **$7,500+** |
| Tool cost | $0 | $15–30/mo |

Cutting delivery time roughly in half doesn't make the work easier — **it raises your ceiling by more than double.** That's the single biggest lever in this plan, and it costs about 1–2% of revenue.

---

## The tool: Vizard

Current reviews put **Vizard** as the best fit for B2B webinar work specifically:

- Built around a **transcript-first editor** — the same read-don't-scrub workflow the spec already calls for
- **Granular brand control** — exact hex codes, fonts, drop shadows. That matters when you're running multiple clients and each needs to look like themselves
- Reviewers report generating a month of shorts from one long recording with only minor text corrections
- **~$15/mo annual, ~$30 for advanced tiers** without watermarks
- API access from the Creator tier if you ever automate the pipeline

**Also worth a look: Choppity** (~$20/mo). It's the only one combining clip generation with **posting, scheduling, and per-post analytics** in one product. Since your retainer promises a distribution calendar and monthly reporting, that could collapse three tools into one.

**OpusClip** (~$15/mo) is the most popular and the most hands-off, but its templates are more "viral creator" than brand-controlled, and API access is locked behind custom pricing.

Start with Vizard's free tier. Run one webinar through it before you pay anything.

---

## ⚠ The limitation that actually matters

Testing across tools finds roughly **90% accuracy on single-speaker talking-head content** — and a sharp drop-off with multiple speakers, screen-share, or slide-heavy material. Tools "struggle with screen-share-heavy webinar recordings where there is no clear speaker to frame."

**That's a large share of B2B webinars.**

A webinar that's 45 minutes of slides with a voiceover is bad for AI tools *and* bad for vertical social generally — you cannot build a compelling 9:16 clip out of a slide deck.

### So add one qualifier to prospecting

> **Does their webinar show a presenter on camera, or is it all screen-share?**

Check this before you log a prospect. Ninety seconds, and it saves you from selling a service you can't deliver well. Prefer:

- ✅ Webcam or studio presenter, visible for most of the runtime
- ✅ Two-person interview format with speaker switching
- ⚠️ Presenter in a corner with slides dominating — workable, more manual effort
- ❌ Pure screen-share with voiceover — **skip it**

This belongs in `Prospect_List.md` alongside the other filters.

---

## The revised pipeline

```
1. INTAKE      client drops recording           →  client-side
2. UPLOAD      into Vizard                      →  5 min
3. GENERATE    AI proposes 20–30 clips          →  automated
4. REVIEW      you pick the 10–16 that are good →  15 min  ◄── keep this
5. CORRECT     fix captions, names, jargon      →  20 min
6. BRAND       apply the client's template      →  automated
7. EXPORT      batch                            →  5 min
8. DELIVER     shared folder + schedule         →  20 min
```

**~65 minutes per batch.** Compare to eight hours by hand.

### Keep step 4

Not out of craft precious-ness. Because reviewing 20 AI-suggested clips and choosing the best 10 takes fifteen minutes and is the entire difference between "clips" and "good clips." AI finds speech boundaries; it doesn't know what's interesting. That review is the cheapest quality control available, and it's the part of the job that's actually yours.

### Keep Final Cut as the fixer

You own it, it's free, and roughly one clip in ten will come out of any AI tool with a bad crop or an awkward cut. Fix those by hand rather than shipping them. Vizard has its own editor too — use whichever is faster once you know both.

---

## Know what you're selling

If the tool does the cutting, a client could cancel and buy Vizard themselves for $30. That's a real risk and you should be clear-eyed about it.

**Your product isn't the editing.** It's that they won't do it. Consistent output every month, brand setup handled, captions proofread, scheduling done, a report at month end, and zero thinking required from them. That's a legitimate business — most service businesses are exactly "I do the thing you won't" — but it means:

- **Don't sell "video editing."** Sell *"your webinar library, working."*
- **Bundle beyond the clips.** Distribution calendar and reporting are what a $30 tool doesn't give them.
- **Expect price pressure eventually.** Some client will figure out the tool exists. The answer isn't to hide it, it's that they still don't want to run it every month.

---

## What changes elsewhere

| File | Change |
|---|---|
| `Operating_Flow.md` | Delivery drops to ~5 hrs/client/month. Ceiling rises from 2 clients to 5. |
| `Prospect_List.md` | Add the on-camera-presenter check to qualifying |
| `Asset_Template_Spec.md` | Still governs the *look* — safe zones, caption style, structure. Build it as a Vizard brand template instead of a Final Cut project. |

The spec doesn't become irrelevant. It becomes the brief you feed the tool.

---

## This week

1. Vizard free tier, run one conference talk through it
2. Compare the output against the spec — does it hit the safe zones and caption rules?
3. Build one brand template from what you learn
4. Pick your demo clip from the results and clean it up
