---
tags:
  - ai-tools
  - content-repurposing
  - video-editing
  - social-media
  - content-marketing
  - opusclip
category: consulting
created: 2026-05-27
language: en
summary: Step-by-step guide to using OpusClip to repurpose one long video (webinar, podcast, interview, training) into many captioned, reframed short social clips — covering plan limits, pre-generation settings that save credits, the editor, and export options.
---

# Turn Long Videos Into Social Clips With OpusClip

Repurpose existing long-form video instead of recording new content. OpusClip auto-detects key moments, reframes to vertical/square/landscape, and adds captions — turning a webinar, podcast, interview, or training recording into a batch of short clips in minutes. Always review each clip before publishing: auto-captions and auto-reframing are good but not perfect.

*(Guide source: Igor Pogany / AIA Team, "Head of AI Education". Level: Navigator.)*

---

## Key Points

- **Repurpose, don't recreate** — one long video already holds dozens of clip-worthy moments.
- **Don't hit "Get clips in 1 click" immediately** — review settings first; the right settings (especially **Processing timeframe**) save credits and improve quality.
- **1 credit ≈ 1 minute** of video analyzed. Trim irrelevant intro/outro and pre-cut filler to spend fewer credits.
- **Always review output** — fix caption errors (accents, jargon, abbreviations) and odd auto-reframes manually.
- **Changes aren't saved unless you click Save** (or enable Auto-save).

---

## Plan Limits (Free vs. Paid)

| | Free Forever | Starter / Pro |
|---|---|---|
| Credits | 60/month (1 credit ≈ 1 min) | Higher tiers |
| Auto reframe + captions | Yes | Yes |
| Manual editing | **No** | Yes |
| Watermark | Yes | No |
| Clip export window | Expires after 3 days | Persistent |
| Upload sources | Local drive, YouTube | + Google Drive, Vimeo, Zoom, Twitch, LinkedIn, etc. |

Full manual editing requires Starter or Pro. (This guide assumes a Pro account so all features are visible.)

---

## Workflow

### 1. Create an account
OpusClip site → **Sign in / Sign up** → log in with Google / Apple / Facebook / email → land on the Dashboard.

### 2. Add the video
From the Dashboard, upload a local file or paste a YouTube link (Pro adds Drive, Vimeo, Zoom, Twitch, LinkedIn, etc.). OpusClip analyzes it. **Do NOT click "Get clips in 1 click" yet.**

### 3. Review settings before generating
Under **AI Clipping** (or use the **Don't Clip** tab if you only want captions, no clips):

- **Clip model** — `Auto` (let it choose), `ClipAnything` (general content), `ClipBasic` (talking-head).
- **Genre** — the content type (podcast, tutorial, etc.) so it knows what moments to hunt for. Click the **cogwheel** after picking a genre to fine-tune selection (high-emotion moments, top highlights, best-of compilation).
- **Clip length** — from <30s up to 10–15 min. Match to where you'll publish.
- **Auto hook** — auto-adds an attention-grabbing text hook to the top 10 clips.
- **Prompt box** — tell it *what topic/moments* to focus on (e.g. "compile the moments about the ChatGPT updates"). Distinct from Genre fine-tuning, which controls *style*.
- **Processing timeframe** — *the key credit saver.* Defaults to the whole video (1 credit/min); restrict to a section to spend less. Exclude irrelevant start/end.
- **Quick presets** — caption style + visual layout (font, color, position). Custom templates/brand kits live under **My Templates**.
- **Aspect ratio** — `9:16` vertical (TikTok, Reels, Shorts), `1:1` square, `16:9` landscape (LinkedIn, YouTube). Options depend on plan.

Only **after** choosing settings, click **Get clips in 1 click**. It shows the credit cost before you confirm.

### 4. Wait
Processing time depends on video length, plan, and server load. You get an email when clips are ready.

### 5. Review generated clips
Click the video preview on the Dashboard to see all clips. The first 10 may carry an **Auto hook** (white-background phrase shown only at the start). Each clip gets a **Viral Score** (0–100, predicted performance). Mark keepers as **Favorite** — hover → heart icon (top-left). Favorites collect under the **Favorite clips** tab.

### 6. Edit a clip (the Editor)
Select a clip → **Edit clip** (scissors icon, lower right). Skip to step 7 if you're happy as-is.

Layout: transcript on the left (highlighted words colored), timeline at bottom, options top + right-side menu.

- **Transcript** — click any word to jump the video there; fix spelling, change highlighted words, add/delete segments via the per-word menu.
- **Timeline** — a clip may be one segment or several. Right-click the bar above the timeline to change a segment's layout; split larger segments.
- **Layout / Tracker** (above the preview) — **Tracker** locks onto an object/speaker and keeps it centered as it moves. Click the subject; OpusClip selects the whole object.

Right-side menu:

- **AI enhance** — remove filler words, remove pauses, auto-censor words, etc.
- **Captions** — swap presets or manually set font/size/color/effects; drag to reposition.
- **Media** — upload your own images/video/audio.
- **Brand Template** — save settings as a reusable brand kit.
- **B-Roll** — replace footage with stock or AI-generated segments (auto or prompt-driven). *No extra credit cost*, but daily prompt limits apply by plan. (*B-roll = supplemental footage intercut with the main "A-roll" for context/interest, e.g. cutaways in an interview.*)
- **Transitions** — segment-to-segment transition style.
- **Text** — add a text field.
- **Music** — royalty-free tracks or your own upload.
- **AI hook** — voice-over hook: write the script, pick voice + tone, generate.

**Save manually** (button at top) or enable **Auto-save** from the Dashboard — edits are otherwise discarded.

### 7. Export / publish
**Export** (top right) → three options:

- **Publish on Social** — connect accounts, schedule/publish directly from OpusClip.
- **Export XML** — original video + `.XML` (preserves edits) + `.SRT` (captions) for pro editors.
- **Download HD** — `.MP4` to your machine to upload anywhere.

---

## Worked Examples

- **Long → short, full workflow** — 26-min raw recording = 26 credits. Used ClipAnything, 30–59s clips, Auto hook on, "Talking head & Speech" genre, prompt "compile the moments where Igor talks about the ChatGPT updates", a caption preset, 9:16. Result: 28 clips, best 10 with AI hooks. Then trimmed pauses/repeats via transcript + AI enhance, dropped in B-roll, exported.
  - **Credit-saving tip:** before generating, open the Video editor (uploads up to 1 GB / 120 min), run **AI enhance → remove pauses/filler** to shorten the source — every minute cut saves a credit.
- **16:9 → 9:16 vertical** — for a single speaker it reframes to keep them in frame; for two speakers (e.g. a podcast) it stacks one on top and one on the bottom automatically. **AI Enhance → Speaker colors** gives each speaker their own caption color.

---

## Other Features

- **OpusClip Thumbnail** (Beta) — AI-generated thumbnail from your video/link; optionally upload your face. Profile menu (top left).
- **Scheduler** — left menu calendar; **Schedule post** to publish uploads, Projects, or Favorites at a chosen time (requires linked social accounts).
- **Analytics** (Beta) — currently TikTok/YouTube stats only; more planned.

---

## Related

- [[business-streamlining-playbooks]] — content repurposing is a natural playbook candidate for an AI consulting/content practice.
- [[playbooking-method]] — wrap this tool workflow as a four-component playbook (trigger, inputs, steps, outputs) to run it repeatably.
