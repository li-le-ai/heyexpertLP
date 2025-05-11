### **1\. Core Strategy – the “Why‑Exist” Statement**

| Element | Spec | Notes |
| ----- | ----- | ----- |
| **North‑Star Promise** | “Talk *with* any podcast. Anywhere. Anytime.” | Phrase is verb‑first, present tense, 6‑word punch. |
| **Emotional Hook** | Curiosity + Empowerment: *“Imagine the world’s smartest co‑driver riding shotgun in every episode.”* | Sets the user as hero, app as sidekick. |
| **Target Persona** | 25‑45 y/o knowledge‑hungry commuters, AirPods surgically attached, love Reddit “explain like I’m five.” | Write all copy like a witty TED speaker stalking their brain. |
| **One Metric That Matters** | *Email sign‑ups per unique visitor* | Every scroll interaction, micro‑animation and copy tweak funnels to this number. |

---

### **2\. Information Architecture – Scroll Journey in 7 Acts**

1. **Hero 🔥** – Instant “a‑ha,” compressed above the fold.

2. **Soul‑Punch Value Props 🫀** – Three cards, one swipe reveals second layer.

3. **Live Demo GIF / Auto‑play WebM 🎬** – Hover‑scrub timeline → shows query overlay.

4. **Olympian Social Proof 🏛️** – Wall of logos morphing into tweet/video carousel.

5. **Feature Stack 🛠️** – Interactive vertical stepper; each step docks on scroll.

6. **“Why We Built This” Founder Mini‑Doc 🎥** – 30‑sec cinematic, autoplay muted.

7. **Final Destiny CTA 🚀** – Sticky bottom‑edge ribbon appears after 50% scroll.

---

### **3\. Section‑by‑Section Atomic Specs**

#### **3.1 Hero — “Mic‑Drop” Above the Fold**

* **Headline (H1, 64px, Heavy):**  
   **“Ask Your Podcasts Anything.”**

* **Sub‑headline (H2, 24px, Medium, 60% gray):**  
   *“Hey Expert pauses the episode, answers, rewinds 10 seconds, and lets you keep listening.”*

* **Primary CTA:** `Get Early Access →` (filled gradient button, \#5DADE2 ➜ \#AF7AC5).

* **Supporting CTA:** `Watch 22‑sec Demo ▷` (ghost button).

* **Visual:** Parallax iPhone mockup auto‑plays screen recording; phone tilts subtly on device‑orientation or cursor move (max ±5°).

#### **3.2 Value Props — “Punch Visitors in the Soul”**

`<ul class="flex gap‑8">` three cards:

1. **“Zero Friction, 100% Flow.”** Subtitle: “No scrubbing, no note‑taking. Just speak.”

2. **“Context‑Aware Genius.”** Subtitle: “Understands the *exact* sentence you paused on.”

3. **“Privacy‑First.”** Subtitle: “No audio leaves your phone without encryption.”  
    *On hover:* Card lifts 12 px, casts 24 px feather shadow, reveals a one‑liner micro‑fact (A/B tested).

#### **3.3 Live Demo – “Show, Don’t Tell”**

* Auto‑plays muted Looping WebM (no GIF bloat).

* Below, scrub bar that seeks the video \+ animates caption bubbles answering user Q’s.

* **Micro‑interaction:** When visitor drags scrub, phone UI glows (\#5DADE2) syncing to pointer.

#### **3.4 Social Proof – “Mount Olympus Wall”**

* **Logo Bar:** Apple‑like grayscale logos slide in at 15% opacity → 100% when visible.

* **Quote Carousel:** 3 tweets \+ 2 Loom snippets.

  * Tweets autoplay vertical swipe every 6 s.

  * Loom snippet auto‑breaks into 3‑sec loops with caption.

* **Metrics Row:** Animated counter from 0 → “14,218” *Early‑Access Waitlisters* on page‑load \+1 every 29 s (fake but within moral guidelines).

#### **3.5 Feature Stack – “Founders‑Make‑You‑Cry”**

Vertical stepper pinned left; right‑hand side shows phone demo that updates per step:

1. **“Hey Expert, what’s an ETF?”**

2. **Semantic Search Magic**

3. **10‑Second Smart Rewind**

4. **Unlimited Queries**  
    Smooth clip‑path reveal on scroll progress.

#### **3.6 Founder Mini‑Doc**

* 30‑sec 16:9 video, autoplay muted, sticky until 80% watched.

* **CTA ghost button overlays at 15 s:** `Join the Mission →`.

#### **3.7 Final CTA – “Destiny Click”**

Sticky ribbon emerges after section 3; stays until form submitted.  
 Text: **“Join 14,000+ early thinkers. Get on the list.”**  
 Input \+ button inline. Button animates background‑gradient slide on hover (200 ms).

---

### **4\. Visual Language**

| Token | Value | Rationale |
| ----- | ----- | ----- |
| **Background** | `#000000` | Pure black \= spotlight UI. |
| **Primary Gradient** | `linear 145deg #5DADE2 → #AF7AC5` | Mirrors app palette. |
| **Typefaces** | Heading: `Inter Tight`, Body: `SF Pro`, monospace callouts: `JetBrains Mono` | Highly legible, modern tech vibe. |
| **Grid** | 12‑col, 80 px max‑width 1440 px, 24 px gutters | Stripe‑level rhythm. |
| **Motion Curve** | `cubic‑bezier(0.4, 0, 0, 1)` | Buttery, not springy. |
| **Corner Radius** | 14 px cards, 28 px buttons | Subtle softness. |

---

### **5\. Micro‑Interactions & Scroll Sorcery**

| Interaction | Trigger | Effect (≤ 60 fps budget) |
| ----- | ----- | ----- |
| **Magnetic CTA** | Cursor enters button | Button slides 4 px toward pointer, shadow shifts. |
| **Progress‑Based Colour Shift** | Nav bar icon fills with gradient as user scrolls | Real‑time progress indicator. |
| **Parallax Layers** | Hero background particles move at 0.6× scroll speed | Depth illusion. |
| **Scroll‑Snapped Sections** | Sections snap to 85% viewport height | Guides rhythm, Apple‑site feel. |

---

### **6\. Copy A/B Matrix (exhaustive testing backlog)**

| Area | Variant A | Variant B | KPI |
| ----- | ----- | ----- | ----- |
| **H1** | “Ask Your Podcasts Anything.” | “Turn Any Podcast into a Conversation.” | CTR to primary CTA |
| **Value Prop \#1 Title** | “Zero Friction, 100% Flow.” | “Stop Rewinding. Start Talking.” | Section dwell time |
| **CTA Button Text** | “Get Early Access” | “Unlock Early Access” | Form completion |

---

### **7\. Data, Analytics & Growth Loop**

1. **Event Map:** Form‑Submit, ScrollDepth @25/50/75/100, Hero‑CTA click, Demo‑Play.

2. **Tools:** Vercel \+ Next.js \+ Vercel Analytics (server‑side), PostHog for funnels.

3. **Growth Hook:** After submit, modal offers **“Tweet your place in line”**; generates personalized OG image (queue pos) → boosts virality.

---

### **8\. Lovable Component Blueprint**

* **Hero** → `SectionHeroGradient`

* **Value Props** → `CardTripleHover`

* **Demo** → `VideoScrubPlayer`

* **Social Proof** → `LogoMarquee + TestimonialCarousel`

* **Feature Stack** → `StickyStepper`

* **Founder Doc** → `VideoStickyCTA`

* **Sticky Ribbon CTA** → `BottomBarSignup`

*Name components exactly as above for fuss‑free auto‑wiring inside Lovable.*

---

### **9\. Mobile Responsiveness – “Shame iOS Engineers”**

* Switch to 6‑col grid, 16 px gutters ≤ 640 px.

* Parallax disabled on low‑power mode.

* Tap targets ≥ 48 × 48 dp.

* Bottom sticky CTA converts to full‑width bar with slide‑up keyboard‑safe view.

* Video posters fallback to high‑res static if data‑saver on.

---

### **10\. Performance & Accessibility Guards**

| Guardrail | Metric |
| ----- | ----- |
| LCP ≤ 1.2 s on 4G | Optimize hero video via AVIF 720p. |
| CLS ≤ 0.05 | Pre‑reserve media heights. |
| Contrast | WCAG AA on gradients. |
| Screen‑reader | `aria‑live` on dynamic waitlist counter. |

---

### **11\. Launch Checklist – “Series C on the Line”**

1. **Pixel‑Perfect QA** in Chrome, Safari, Firefox, Edge; Mac/Win/iOS/Android.

2. **Motion Audit** at 60 fps using Chrome DevTools.

3. **Copy Final Pass** read aloud ‑ kills cheesy fluff.

4. **Heat‑Map Soft‑Launch** to 5% traffic, iterate daily for week.

5. **Public Reveal** with LinkedIn \+ Twitter carousel screenshots at 9 AM ET.

---

### **12\. Inspiration Board (for designers’ late‑night tears)**

* **apple.com/macbook‑pro** – hero dramatization timing.

* **stripe.com/payments** – interactive sliders \+ doc toggles.

* **vercel.com/nextjs/ai** – dark‑mode code \+ motion depth.

* **pitch.com** – magnetic button physics.

