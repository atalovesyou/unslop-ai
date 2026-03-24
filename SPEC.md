# UnSlop.ai — Product Spec

## One-Liner
**Kill the AI slop.** Paste any text → get a slop score + humanized version.

## Problem
AI-generated content is everywhere: blogs, emails, LinkedIn posts, product descriptions. It all sounds the same — vague, wordy, over-hedged, full of "delve," "leverage," "in today's fast-paced world." People hate reading it. Google is starting to penalize it. But most people can't tell *what specifically* makes their text sound AI-generated, or how to fix it.

## Solution
1. **Slop Score (0-100):** Paste text, get an instant slop rating with breakdown (filler words, hedging, AI clichés, passive voice, corporate jargon)
2. **De-Slop It:** One-click rewrite that preserves meaning but removes AI-ness
3. **Chrome Extension:** Highlight AI slop on any webpage in real-time
4. **API:** For content teams and publishers to filter at scale

## Target Users
- Content marketers who use AI but want to sound human
- SEO professionals worried about Google's helpful content update
- Publishers and editors screening submissions
- LinkedIn posters tired of sounding like ChatGPT
- Students worried about AI detection (adjacent use case)

## Competitive Landscape
- **GPTZero, Originality.ai, ZeroGPT** — AI *detectors* (binary: AI or human). Different angle — they detect, we *fix*.
- **Hemingway Editor** — General writing improvement. Not AI-specific.
- **Undetectable.ai** — Makes AI text bypass detectors. Sketchy/adversarial. We're the *opposite* — make text genuinely better.
- **No direct competitor** combines detection + scoring + rewriting specifically for AI slop.

## MVP (Ship in 1 week)
- Landing page (Next.js or static)
- Text input → Slop Score (API call to Claude/GPT with slop-scoring prompt)
- One-click de-slop rewrite
- Email capture for Chrome extension waitlist
- Free tier: 5 de-slops/day, paid: unlimited

## Tech Stack
- **Frontend:** Next.js + Tailwind (or even simpler: single HTML page with JS)
- **Backend:** Vercel serverless functions or Cloudflare Workers
- **AI:** Claude API for scoring + rewriting (or Atal's Ollama for cost savings)
- **Domain:** unslop.ai (need to check/register)

## Monetization
- **Free:** 5 scans/day
- **Pro:** $9/mo — unlimited scans + Chrome extension + API access
- **Team:** $29/mo — team dashboard, bulk processing
- **API:** Usage-based pricing for publishers

## Marketing Angle
- "Your content doesn't have to sound like ChatGPT wrote it"
- Launch on Product Hunt, Hacker News, Twitter
- Create a "Slop Score" for famous AI-generated articles/posts as viral content
- LinkedIn post series: "I ran [famous person]'s post through UnSlop.ai and..."

## Revenue Potential
- Low CAC (viral/organic), $9-29/mo subscriptions
- 1,000 paying users = $9-29K MRR
- Content marketing flywheel — the product IS the content
# UnSlop.ai — Landing Page Copy

## Hero Section

### Headline
**Your content reeks of AI. Fix it.**

### Subheadline
Paste any text. Get a Slop Score. One click to sound human again.

### CTA
**[De-Slop My Text →]** (free, no signup)

---

## How It Works (3 steps)

**1. Paste your text**
Blog post, email, LinkedIn update — anything that might sound AI-generated.

**2. Get your Slop Score**
0-100 rating with a detailed breakdown: filler words, hedging, AI clichés, passive voice, corporate emptiness.

**3. One-click fix**
Hit "De-Slop It" and get a rewrite that says the same thing but sounds like a human wrote it.

---

## The Slop Score Breakdown

Your text gets scored across 6 dimensions:

- 🤖 **AI Clichés** — "delve," "landscape," "it's worth noting," "in today's fast-paced world"
- 💨 **Filler & Hedging** — "arguably," "it could be said that," "generally speaking"
- 😴 **Passive Voice** — hiding who does what behind bureaucratic construction
- 🏢 **Corporate Jargon** — "leverage," "synergize," "drive alignment," "circle back"
- 📏 **Sentence Monotony** — every sentence the same length and rhythm (dead giveaway)
- 🎭 **Fake Enthusiasm** — exclamation points on boring statements! Amazing!

---

## Who Needs This

- **Content marketers** using AI tools but wanting human-quality output
- **SEO teams** avoiding Google's AI content penalties
- **LinkedIn creators** tired of sounding like everyone else's ChatGPT
- **Publishers & editors** screening submissions for AI slop
- **Anyone** who writes with AI and has standards

---

## Why Not Just "Edit It Yourself"?

Because you can't see your own slop. It's like trying to smell your own house — you're nose-blind to it. UnSlop.ai catches patterns you'd never notice:

> **Before (Slop Score: 87/100):**
> "In today's rapidly evolving digital landscape, it's worth noting that leveraging AI-powered solutions can arguably help businesses navigate the complexities of content creation. By embracing innovative approaches, organizations can drive meaningful engagement and foster authentic connections with their target audience."

> **After (Slop Score: 12/100):**
> "AI can help you write faster. But if every sentence sounds like a press release, nobody reads past the first paragraph. Write like you talk. Cut the jargon. Say something specific."

---

## Pricing

**Free** — 5 scans/day. No signup needed.

**Pro — $9/mo**
- Unlimited scans
- Chrome extension (highlight slop anywhere)
- Tone presets (casual, professional, academic)
- API access (1,000 calls/mo)

**Team — $29/mo**
- Everything in Pro
- Team dashboard
- Bulk processing (upload CSV/docs)
- Style guide enforcement

---

## FAQ

**Is this an AI detector?**
No. AI detectors tell you "this is AI." We tell you *why it sounds like AI* and fix it. We're not here to catch cheaters — we're here to make writing better.

**Does it work for non-English?**
Not yet. English only for now. More languages coming.

**What AI model do you use?**
We use a combination of pattern matching (for scoring) and large language models (for rewriting). The scoring is deterministic, not vibes-based.

**Will my text be stored?**
No. We process and forget. Your text is never stored or used for training.

---

## Footer CTA
**Stop sounding like ChatGPT.**
[De-Slop My Text →]

---

## Meta
- **Title tag:** UnSlop.ai — Kill the AI Slop in Your Writing
- **Meta description:** Paste any text, get a Slop Score (0-100), and one-click rewrite it to sound human. Free AI content fixer.
- **OG image:** Before/after comparison with slop scores
