# Portfolio Design System

Sync note: keep `DESIGN.md` and `.context/design-brief.md` byte-for-byte identical when editing the design direction.

## Read

The current site is visually committed: black cyber-grid world, animated scan fields, orbit rings, ticker tape, color-changing chapters, neon accents, huge uppercase Inter Tight headings, and hover-heavy proof cards.

That makes the page memorable, but it slightly overstates the wrong signal for the target audience. The likely reader is a founder, CEO, investor, or senior hiring manager evaluating Chief of Staff, Strategy/Growth, Founder Office, and 0-to-1 operating roles. That audience wants evidence of judgment, executive trust, clarity under ambiguity, and commercial ownership. The cyber/kinetic language says "builder/hacker/AI-native" loudly, but can make the portfolio feel more like a tech demo than a senior operator's proof surface.

Verdict: keep the kinetic operating metaphor, but de-cyber it. The site should feel like a high-conviction operator memo with selective motion, not a sci-fi dashboard.

## Recommended Direction

Direction: **Executive Operator Editorial**

The tighter design should combine:

- Strategic memo clarity
- Founder-office pace
- Measured visual tension
- Strong numerical proof
- A small AI-native edge, used as accent rather than identity

Memorable thing: **Arun turns ambiguous growth bets into operating systems that scale.**

Everything on the page should support that idea. The current "Chaos to Scale" thesis is strong and should stay, but it should be expressed with sharper editorial structure and less ambient cyber decoration.

## Design System Contract

This document is the source of truth for visual implementation.

Fixed decisions:

- Aesthetic direction: Executive Operator Editorial.
- First viewport hierarchy: name, role, thesis, proof, actions, then visual world.
- Primary palette: ink/charcoal/panel neutrals with `#4F7CFF` as the identity accent.
- Accent usage: gold, green, and red only for proof/data contexts.
- Typography roles: Satoshi for display, Source Sans 3 for body, IBM Plex Mono for data and metrics. Do not keep one compressed font for every role.
- Motion level: intentional-functional. Motion supports comprehension and never gates proof.
- Cards: only for repeated proof, career, artifact, or human-layer items. No decorative card grids.
- Cyber reduction: remove or heavily reduce scan, orbit, glow-node, ticker, and full-section accent-shift patterns.

Flexible decisions:

- The operating diagram can be abstract, editorial, or blueprint-like, as long as it stays secondary to proof.

Changes that need explicit approval:

- Returning to a neon multi-accent cyber identity.
- Reintroducing a continuous ticker as the primary proof presentation.
- Making the hero visual world more prominent than the role and proof hierarchy.
- Adding new sections before the core proof path is implemented.

Hero visual direction:

- Use a restrained operating diagram as the secondary hero visual.
- The diagram should feel like an executive system map: nodes, flows, proof labels, and light grid lines tied to Strategy, Growth, and Build.
- It may include selected proof labels such as `$20M Series A`, `$2M MRR`, `₹100Cr+ AGWP`, and `500M+ views`.
- It should not use orbit rings, glowing cyber nodes, scan rectangles, or a full sci-fi control-room composition.
- On mobile, the diagram should simplify or disappear after the proof strip. It must never push role, thesis, proof, or actions below the first useful screen.

## What To Keep

- The large hero name. It creates confidence and avoids a generic resume page.
- The "Chaos to Scale" operating thesis. It is the site's best positioning line.
- The proof-first numbers: `$20M`, `$1.5M MRR`, `₹100Cr+`, `500M+`.
- The chaptered career arc. It makes a non-linear career easier to understand.
- Dark mode as the primary canvas, because it makes the portfolio feel decisive and distinct.

## What To Reduce

- Reduce grid, scan, orbit, glowing node, and radial effects by roughly 70%.
- Remove the continuous ticker or convert it into a static proof bar. The ticker adds energy but competes with the actual story.
- Stop changing the whole accent system per chapter. It adds interaction novelty but weakens brand coherence.
- Use fewer all-uppercase blocks. Keep uppercase for labels and proof numbers, not every heading and card.
- Reduce hover lift and animated reveal. The site should feel composed, not constantly in motion.

## Typography

Use this final editorial pairing:

- Display: **Satoshi** for hero, section titles, proof numbers, and primary navigation.
- Body: **Source Sans 3** for paragraphs, case-study copy, career details, and supporting labels.
- Data/metrics: **IBM Plex Mono** for years, ranks, MRR, ARR, DAU, financial figures, and proof metadata.

Avoid using Inter Tight as the entire identity. It gives the current page a compressed, poster-like intensity, but it makes long proof content feel less executive. The new type system separates roles: confident display, readable body, precise metric labels.

Font loading:

- Load Satoshi from a reliable hosted source or self-host it if licensing/assets are available.
- Load Source Sans 3 and IBM Plex Mono from Google Fonts or an equivalent privacy/performance-safe provider.
- Use `font-display: swap`.
- Fallbacks are allowed only as fallbacks, not as the visible design identity.

Suggested scale:

- Hero name: 112-148px desktop, 64-84px mobile, tight but not crushed.
- Section headings: 48-72px desktop, 36-44px mobile.
- Card headings: 20-28px.
- Body: 16-18px with 1.55-1.7 line height.
- Labels: 11-12px uppercase, restrained tracking.

## Section Rhythm

Recommended page rhythm:

1. **Hero:** name, role target, one-line thesis, three proof stats, contact/CV/LinkedIn.
2. **Proof Bar:** static, high-signal metrics with short context under each.
3. **Operating Thesis:** "Chaos to Scale" explained as 3 operating modes: Strategy, Growth, Build.
4. **Career Arc:** timeline or chapter list, but with calmer interaction and clearer chronology.
5. **Selected Proof:** 3 case-study cards, each framed as situation, action, result.
6. **Artifacts / Builder Layer:** compact future shelf after selected proof, explicitly secondary until real artifacts exist.
7. **Human Layer:** compact, warmer, less card-heavy.
8. **Footer:** direct outreach and CV.

Spacing should be generous but not theatrical:

- Desktop section padding: 88-112px.
- Mobile section padding: 56-72px.
- Max content width: 1180-1280px for most sections; only hero can go wider.
- Cards: 8px radius max, thin borders, low-contrast surfaces.

Responsive structure:

- Desktop `1024px+`: hero may use a two-column composition, with text/proof/actions on the left and a secondary operating diagram on the right.
- Tablet `768-1023px`: keep the hero text, proof strip, and actions stacked before any visual diagram. Career arc should become a single-column timeline.
- Mobile `<768px`: first viewport must show name, role, thesis, at least two proof metrics, and one primary action before any decorative visual. Hide or simplify the operating diagram.
- Mobile nav: use a visible 44px minimum menu target, full-width open menu, and dismiss on selection.
- Proof metrics: wrap into a two-column mobile grid or stacked list. Do not use horizontal scrolling or ticker behavior.
- Career chapters: use readable vertical rhythm with logos/text badges sized consistently. No sticky side panel on mobile.
- Footer actions: stack full-width or wrap cleanly with at least 44px height.

First viewport hierarchy:

```text
1. Arun Sharma
2. Chief of Staff / Strategy & Growth / 0-to-1 Operator
3. Turns ambiguous growth bets into operating systems that scale
4. Proof strip: $20M Series A | $2M MRR | ₹100Cr+ AGWP | 500M+ views
5. Primary actions: Contact | Download CV | LinkedIn
6. Subtle operating diagram, not a cyber scene
```

This is a founder-office hierarchy: the visitor should understand who Arun is, what role he fits, and why the proof is credible before they process the visual world. Cinematic treatment still matters, but it should support the proof path rather than compete with it.

## Page Wireframes

These wireframes define structure, not final spacing or copy. Implementation can refine proportions, but it should not change the reading order without explicit approval.

Desktop `1024px+`:

```text
┌────────────────────────────────────────────────────────────────────────────┐
│ NAV: Arun Sharma                         World  Proof  Experience  Contact │
├────────────────────────────────────────────────────────────────────────────┤
│ HERO                                                                       │
│ ┌──────────────────────────────────────┐ ┌───────────────────────────────┐ │
│ │ Arun Sharma                          │ │ Secondary operating diagram   │ │
│ │ Chief of Staff / Strategy & Growth   │ │ Strategy → Growth → Build     │ │
│ │ Turns ambiguous growth bets into     │ │ Proof labels as small nodes   │ │
│ │ operating systems that scale         │ │ No orbit / scan / glow scene  │ │
│ │                                      │ │                               │ │
│ │ $20M Series A | $2M MRR              │ │                               │ │
│ │ ₹100Cr+ AGWP | 500M+ views           │ │                               │ │
│ │                                      │ │                               │ │
│ │ [Contact] [Download CV] [LinkedIn]   │ │                               │ │
│ └──────────────────────────────────────┘ └───────────────────────────────┘ │
├────────────────────────────────────────────────────────────────────────────┤
│ PROOF BAR: static metrics with one-line ownership context                  │
├────────────────────────────────────────────────────────────────────────────┤
│ OPERATING THESIS: Strategy / Growth / Build as one editorial band          │
├────────────────────────────────────────────────────────────────────────────┤
│ CAREER ARC: left timeline + right chapter detail, no heavy visual effects  │
├────────────────────────────────────────────────────────────────────────────┤
│ SELECTED PROOF: 3 deep cases, Mayhem / PocketFM / InsuranceDekho           │
├────────────────────────────────────────────────────────────────────────────┤
│ ARTIFACT SHELF: compact future-facing row, honest coming-soon surfaces     │
├────────────────────────────────────────────────────────────────────────────┤
│ HUMAN LAYER: compact warmth, real interests, no decorative card bloat      │
├────────────────────────────────────────────────────────────────────────────┤
│ FOOTER: direct contact, CV, LinkedIn                                       │
└────────────────────────────────────────────────────────────────────────────┘
```

Tablet `768-1023px`:

```text
┌──────────────────────────────────────────────────────────────┐
│ NAV: Arun Sharma                              Menu / Contact │
├──────────────────────────────────────────────────────────────┤
│ HERO                                                         │
│ Arun Sharma                                                  │
│ Chief of Staff / Strategy & Growth / 0-to-1 Operator         │
│ Turns ambiguous growth bets into operating systems that scale│
│                                                              │
│ Static proof strip, wrapped into two rows                    │
│ [Contact] [Download CV] [LinkedIn]                           │
│                                                              │
│ Secondary operating diagram, simplified and below proof      │
├──────────────────────────────────────────────────────────────┤
│ Proof bar                                                    │
├──────────────────────────────────────────────────────────────┤
│ Operating thesis                                             │
├──────────────────────────────────────────────────────────────┤
│ Career arc as single-column timeline                         │
├──────────────────────────────────────────────────────────────┤
│ Three selected proof cases                                   │
├──────────────────────────────────────────────────────────────┤
│ Compact artifact shelf                                       │
├──────────────────────────────────────────────────────────────┤
│ Human layer                                                  │
├──────────────────────────────────────────────────────────────┤
│ Footer                                                       │
└──────────────────────────────────────────────────────────────┘
```

Mobile `<768px`:

```text
┌──────────────────────────────────────┐
│ NAV: Arun Sharma                Menu │
├──────────────────────────────────────┤
│ HERO                                 │
│ Arun Sharma                          │
│ Chief of Staff / Strategy & Growth   │
│ Turns ambiguous growth bets into     │
│ operating systems that scale         │
│                                      │
│ $20M Series A     $2M MRR            │
│ ₹100Cr+ AGWP      500M+ views        │
│                                      │
│ [Contact]                            │
│ [Download CV] [LinkedIn]             │
│                                      │
│ Optional simplified diagram below    │
│ the proof path, never above it       │
├──────────────────────────────────────┤
│ Proof bar as stacked ownership rows  │
├──────────────────────────────────────┤
│ Operating thesis, no icon grid       │
├──────────────────────────────────────┤
│ Career arc as vertical timeline      │
├──────────────────────────────────────┤
│ Proof case 1                         │
│ Proof case 2                         │
│ Proof case 3                         │
├──────────────────────────────────────┤
│ Compact artifact shelf               │
├──────────────────────────────────────┤
│ Human layer                          │
├──────────────────────────────────────┤
│ Footer actions                       │
└──────────────────────────────────────┘
```

Wireframe acceptance rules:

- The hero proof path must be readable before any decorative diagram.
- The proof bar must be static on every viewport.
- The operating thesis must not become a decorative 3-card icon grid.
- The artifact shelf must stay lower priority than selected proof.
- Mobile must not depend on sticky panels, hover states, horizontal scrolling, or animation to reveal proof.

## Color

Move from multi-neon cyber palette to a restrained executive palette with one sharp accent.

Recommended palette:

- Ink: `#07090D`
- Charcoal: `#101318`
- Panel: `#171B22`
- Hairline: `rgba(255,255,255,0.10)`
- Primary text: `#F5F7FA`
- Secondary text: `#A8B0BD`
- Muted text: `#68717F`
- Accent: `#4F7CFF`
- Warm proof accent: `#D9A441`
- Success/growth accent: `#43B883`
- Critical/venture accent: `#D95868`

Use the blue accent as the portfolio's identity. Use gold, green, and red only inside proof/data contexts. Do not let each career chapter repaint the whole site.

## Motion

Motion level: **intentional-functional**.

Keep:

- Smooth scroll.
- Subtle section reveal once.
- Card hover border-color changes.
- Career chapter active-state transition.

Remove or heavily reduce:

- Infinite orbit rings.
- Scanning rectangles.
- Ticker loop.
- Large glowing motion fields.
- Frequent translate-up card motion.

Motion should help the reader understand the career arc. It should not be the most memorable part of the page.

## Interaction States

The portfolio is static, but it still needs explicit states so trust does not depend on the ideal happy path.

| Feature | Default | Empty / Missing | Error / Fail | Success / Active | Reduced Motion |
|---|---|---|---|---|---|
| Hero proof strip | Static proof metrics visible in first viewport | Hide only the missing metric and preserve spacing | Never depend on animation to reveal proof | Metrics readable within 5 seconds | Static proof bar, no ticker |
| Career arc | Chronological chapter list with one active chapter | If a logo is missing, show a text badge with company or school name | Broken image should not collapse layout | Active chapter uses border, marker, and text emphasis | Active state changes on click/tap or static scroll position |
| Projects / artifacts | Compact secondary shelf after selected proof | Use a warm "coming soon" treatment with no dead links | Missing artifact links should be hidden, not disabled | Live artifacts have clear title, type, and outbound affordance | Static cards, no reveal dependency |
| Mobile nav | Closed by default with clear 44px menu target | N/A | N/A | Open state is obvious, full-width, and dismisses after selection | No animated drawer required |
| CV and contact actions | Contact, Download CV, and LinkedIn visible in hero and footer | N/A | If PDF is unavailable, keep contact and LinkedIn primary | Visited, focus, and hover states are visible | No motion dependency |
| Decorative system | Subtle editorial grid or operating diagram | If decorative assets fail, content hierarchy remains intact | Decoration failure never hides text or proof | Visual treatment supports hierarchy without becoming the subject | Remove scan, orbit, ticker, and large translate animations |

## Accessibility

Accessibility is part of the design direction, not post-implementation cleanup.

- Use semantic landmarks: `header`, `nav`, `main`, `section`, and `footer`.
- Keep one visible `h1` for "Arun Sharma"; section headings should follow a clean `h2`/`h3` hierarchy.
- Body text must be at least 16px and meet 4.5:1 contrast against its background.
- Labels and metadata can be smaller only when they are not required for comprehension.
- Every interactive element needs a visible focus state, not only hover.
- Links must preserve visited vs unvisited distinction where practical, especially external/profile links.
- Touch targets must be at least 44px high/wide on mobile.
- Do not rely on hover to reveal essential information. Tap/click and static states must expose the same proof.
- All company/school logos need meaningful `alt` text, with text fallback if the image fails.
- Respect `prefers-reduced-motion`: remove ticker, scan, orbit, large translate reveals, and looping animations.
- Decorative visuals should be hidden from screen readers.
- Contact, CV, and LinkedIn actions should be reachable by keyboard in the same order they appear visually.

## User Journey

The page should move like a cinematic career world, but every section needs a specific emotional job. The reader should feel increasing trust, not just increasing visual stimulation.

| Step | User does | User should feel | Design support |
|---|---|---|---|
| 1 | Lands on hero | "I know who this is fast." | Name, role, thesis, proof strip, and clear contact actions in the first viewport |
| 2 | Scans proof | "This is commercially real." | Static metrics with short ownership context, not a moving ticker |
| 3 | Reads operating thesis | "There is a method here." | Strategy, Growth, and Build as the operating system behind the career |
| 4 | Moves through career arc | "This arc compounds." | Chronological chapters with calmer active states and visible company/school signal |
| 5 | Opens selected proof | "He owned the hard parts." | Situation, action, result framing for the strongest 3 cases |
| 6 | Checks builder and human layer | "There is a person here." | Compact warmth, real interests, and a restrained future artifact shelf without decorative card bloat |
| 7 | Reaches footer | "The next step is obvious." | Email, CV, and LinkedIn repeated without friction |

Time horizon:

- First 5 seconds: role fit and proof must be self-evident.
- First 5 minutes: the career arc should show a repeatable operating pattern, not a list of jobs.
- Long-term memory: the phrase "chaos to scale" should attach to Arun's proof, not to the cyber visual system.

## Visual System

Replace the cyber-world metaphor with an operating-room/editorial system:

- Thin dividers and rule lines.
- Static proof strips.
- Timeline markers.
- Dense but readable case-study panels.
- Small monospaced metadata.
- Occasional blueprint-like grid lines at 5-10% opacity, not across every section.

The site can still feel modern and AI-native, but through precision: structured metrics, operating diagrams, crisp case-study framing, and selective interaction.

## Anti-Slop Rules

The redesign should not become a generic dark SaaS template. Use these rules as implementation guardrails:

- No decorative 3-column feature grid as a primary section. Strategy, Growth, and Build can exist, but they should read as an operating thesis, not icon cards.
- No icons in colored circles as decoration. Icons should clarify actions or section type, not fill empty space.
- No centered-everything section rhythm. Hero and footer may center selectively, but proof, career, and case-study sections should use editorial alignment.
- No card inside card patterns. Use cards only for genuine repeated items: proof cases, career chapters, artifacts, and human-layer items.
- No uniform large border radius. Keep cards at 8px or less, with sharper proof and editorial surfaces.
- No decorative blobs, orbit rings, scan fields, or glow nodes as primary identity. A faint editorial grid or operating diagram is enough.
- No motion that asks the reader to wait before understanding proof. Animation can reveal emphasis, not hide meaning.
- No repeated mood headlines. Each section needs one job: proof, method, arc, artifact, human, or contact.
- No placeholder project links. Future artifacts should be honest "coming soon" surfaces until real work exists.
- No default typography fallback as the visual identity. Fonts must be loaded intentionally and assigned by role.

## Content Framing

The current copy is strong but sometimes too slogan-like. Shift more sections toward proof logic:

- Claim: "Closed $20M Series A"
- Context: "Mayhem Studios spin-off from MPL"
- Role: "Owned investor tracker, pitch deck, VDR, demos, diligence"
- Outcome: "150+ funds pitched, Tier 1 investors closed"

This makes the design feel more senior because the reader can quickly verify the level of ownership behind each headline.

Selected proof cases:

1. **InsuranceDekho: P&L Build**
   - Metric: `₹100Cr+ AGWP`
   - Title: `Built a profitable cross-sell business from zero`
   - Situation: InsuranceDekho had a large agent network but needed new high-margin product lines and sharper distribution monetization.
   - Action: Led cross-sell and financial services GTM, managed a 75+ member execution team, integrated recommendation-led selling, and reported directly into the CEO.
   - Result: Scaled cross-sell to `₹100Cr+ AGWP` and `~₹15Cr ARR` across four high-margin product lines, while supporting agent growth from 80K to 200K+.
   - Tags: `P&L`, `Cross-sell`, `Agent network`, `CEO reporting`
2. **PocketFM: Revenue Growth**
   - Metric: `$2M MRR`
   - Title: `Scaled micro-drama from launch motion to revenue engine`
   - Situation: PocketFM's micro-drama vertical needed fast market entry, repeatable content optimization, and efficient paid/organic GTM.
   - Action: Led a 40-member cross-functional team, built an AI-assisted promo cracking engine, diagnosed listener drop-offs, re-edited shows, and owned paid growth across Meta and Google.
   - Result: Scaled the vertical to `$2M MRR` and 500K DAU in 5 months, while building PocketTV social channels to 500M+ organic views.
   - Tags: `Revenue`, `AI-assisted GTM`, `Content growth`, `Paid + organic`
3. **Mayhem / MPL: Capital Formation**
   - Metric: `$20M Series A`
   - Title: `Turned a studio spin-off into a funded venture`
   - Situation: Mayhem Studios needed to separate from MPL with a credible investor story, diligence process, and GTM path.
   - Action: Owned the investor tracker, pitch deck, VDR, product demos, MIS, diligence support, and fundraise operating rhythm with the CEO.
   - Result: Pitched 150+ global funds, reached 10+ IC conversations, closed a `$20M Series A` from Tier 1 investors including Sequoia Capital, Truecaller, Hashed, and Steadview.
   - Tags: `Capital`, `Spin-off`, `Investor process`, `Gaming`

Use `500M+ organic views` as supporting evidence inside the PocketFM case or proof bar, not as a fourth equal case-study card.

Artifact shelf rules:

- Keep artifacts as one compact row or band after selected proof.
- Label the section as future-facing builder output, not as current proof.
- Do not use fake links, disabled buttons, or oversized placeholder cards.
- If no real artifact links exist, use honest "coming soon" surfaces with one sentence of context.
- When artifacts become real, each item needs a title, type, status, and clear outbound affordance.
- The artifact shelf should never compete visually with the three selected proof cases.

## Final Recommendation

The cyber/kinetic style helps with memorability and signals AI-native energy, but it hurts executive trust when used as the dominant identity. The better direction is not conservative corporate minimalism. It is a calmer, sharper, proof-led editorial portfolio with one controlled accent color and motion reserved for comprehension.

Design target: **a founder should feel "this person brings order, velocity, and commercial judgment" within 10 seconds.**
