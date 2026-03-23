# LinkedIn Profile Update — Full Spec

## Context
Nahuel's LinkedIn is outdated: generic headline, weak about section, Mailberry missing entirely, Snowflake blank, skills dominated by PHP/jQuery. This spec contains the exact copy for every section to be applied via Chrome browser automation.

## Reference: Experience Form Fields
Each experience has: Title, Employment type, Company, Currently working checkbox, Start/End date, Location, Location type, Description (2,000 char max), Skills (up to 5 per role), Media.

---

## 1. HEADLINE

**Current:** `Software Engineer`

**Proposed options (pick one):**

**Option A (Recommended):**
```
Senior Product Engineer | React, TypeScript, Node.js | Building AI-Powered Products
```
(82 chars — fits in search preview, hits key search terms)

**Option B:**
```
Senior Fullstack Engineer | Frontend & UX | React, TypeScript, AI | Ex-Snowflake
```
(81 chars — leverages Snowflake brand recognition)

**Option C:**
```
Founding Engineer at Mailberry | React, TypeScript, Node.js | AI & Frontend/UX
```
(79 chars — leads with current startup role)

---

## 2. ABOUT SECTION

**Current:** "I was born in Spain but currently living and working remotely from Argentina and all around the world. I love technology in general and I'm obsessed with UX and best practices in particular. In my spare time i do ECU (engine management systems) tuning for motorsports."

**Proposed (2,600 char max — first ~300 chars before the fold are critical):**

```
I build products people actually enjoy using. 15+ years shipping web applications — from building a framework adopted across OLX (317M monthly users) to architecting Streamlit's Cloud Platform from scratch (acquired by Snowflake for $800M) to now leading frontend and AI integrations at an early-stage startup.

I'm a fullstack engineer with a sharp frontend eye. My sweet spot is taking complex systems and making them feel simple — whether that's a real-time email editor with 18 custom extensions, a communication layer between Kubernetes and embedded iframes, or a multi-agent AI orchestration dashboard.

Currently at Mailberry as Founding Engineer, building an AI-native email platform for eCommerce. I rebuilt the entire frontend foundation (monorepo architecture, design system, TypeScript strictness) and now ship features across React, Node.js, and AWS while integrating AI from Anthropic, OpenAI, and Google.

What I work with daily: React, TypeScript, Node.js, Tailwind CSS, Vite, Prisma, PostgreSQL, AWS (Lambda, S3, SQS), Vercel AI SDK.

Previously: Snowflake (3 yrs), Streamlit (early engineer → $800M acquisition), Raven[Ops] (robotics/AI), OLX/Naspers (global classifieds, Berlin).

Born in Spain, based in Argentina, working remotely with teams worldwide. Outside of code, I tune Ford Ranger ECU systems for motorsports and run a premium automotive parts import business.

array.dude@gmail.com | github.com/arraydude

React · TypeScript · Node.js · Tailwind CSS · AWS · AI/ML · Vite · Prisma · PostgreSQL · System Design · UX · Technical Leadership · Python · Go · Kubernetes
```

(~1,550 chars — well within 2,600 limit)

**Why this works:**
- First 300 chars hook: "I build products people actually enjoy using" + concrete results (OLX scale, Streamlit acquisition)
- Names specific technologies for SEO
- Quantified impact throughout
- Personal touch at the end (ECU tuning, Tribe Shipping)
- Email for recruiter contact
- Keyword list at the bottom for search indexing

---

## 3. EXPERIENCE — ADD MAILBERRY (new entry)

**Title:** Senior Product Engineer
**Employment type:** Full-time
**Company:** Mailberry
**Currently working:** ✅ Yes
**Start date:** April 2025
**Location:** Los Angeles, California (or leave blank)
**Location type:** Remote

**Description (2,000 char max):**
```
Founding engineer at an AI-native email service provider for eCommerce — building the platform that replaces Mailchimp and Klaviyo with AI-powered automation.

Rebuilt the entire frontend foundation on day one:
• Migrated multi-repo → monorepo architecture
• Replaced Mantine with shadcn/ui, migrated Next.js → Vite
• Created the Design System from scratch (Tailwind v4 + shadcn + Lucide), consumed across all frontend apps
• Enforced TypeScript strictness, ESLint flat config, and CI/CD safety checks on PRs

Built a production-ready TipTap-based email template editor — 67 TypeScript files, 18 extensions, 7 React Email node types with real-time preview editing and full email client compatibility.

Established AI-assisted development standards for the engineering team — created Claude Code skills, agents, and commands that standardize how we build and review code.

Currently building email automation flows (Autopilot) with AI-powered content generation using Vercel AI SDK integrating Anthropic, OpenAI, and Google GenAI.

Stack: React 18, TypeScript, Vite, Tailwind CSS v4, XState, TipTap, Tanstack Query, Node.js, Express, Prisma, PostgreSQL, DynamoDB, AWS (Lambda, S3, SQS, EventBridge), Vercel AI SDK, Stripe, SendGrid, PostHog.
```
(~1,100 chars)

**Skills (5):** React.js, TypeScript, Node.js, Tailwind CSS, AI/ML

---

## 4. EXPERIENCE — EDIT SNOWFLAKE (currently blank)

**Title:** Software Engineer (keep as-is)
**All other fields:** keep as-is

**Description:**
```
Joined via Streamlit acquisition ($800M). Transitioned through three phases: maintaining the standalone Streamlit product → integrating Streamlit into the Snowflake ecosystem (Streamlit-in-Snowflake) → contributing to the main Snowflake web client across multiple areas of the platform.

Worked on both frontend (TypeScript, React) and infrastructure, expanding scope from the original Streamlit codebase to Snowflake's global web application serving enterprise data teams worldwide.
```
(~470 chars — kept shorter since we're still awaiting Nahuel's detailed input from his ex-coworker's PR list. Can be expanded later.)

**Skills (5):** TypeScript, React.js, Python, System Design, Full-Stack Development

---

## 5. EXPERIENCE — EDIT STREAMLIT

**Current description:** "Streamlit is the first app framework specifically for Machine Learning and Data Science teams. Going from the back-end side using Python 2 / 3 to the front-end side using TypeScript / ReactJS."

**New description:**
```
Early engineer at the open-source framework for building data science web apps (raised $62M from Sequoia Capital, GGV Capital). Acquired by Snowflake for ~$800M in 2022.

• Started on the core open-source framework (Python + React), then built the entire Cloud Platform frontend from scratch when the company launched its hosted deployment product
• Designed the communication architecture between Kubernetes → hosted Streamlit apps → iframe embedding → PostMessage/WebSocket layer, strongly typed end-to-end — the critical bridge that made cloud hosting work
• Grew with the company from a small team to acquisition, seeing the platform scale to 8M+ downloads and 1.5M+ apps built
• Translated #30DaysOfStreamlit to Spanish — self-proposed community initiative to expand reach in the Spanish-speaking developer community

Stack: TypeScript, React, SWR, Python 2/3, Go, Tailwind CSS, Kubernetes, WebSockets, Jest, Cypress.
```
(~830 chars)

**Skills (5):** TypeScript, React.js, Python, Kubernetes, WebSocket

---

## 6. EXPERIENCE — EDIT RAVEN[OPS]

**Current description is decent, but can be improved.**

**New description:**
```
First remote role for the US market at an Accel-backed ($3.5M) robotics DevOps startup. Built an intuitive web interface to visualize datasets for robotics — enabling QA teams to visualize, tag, and iterate AI model data faster.

• Synced video playback of robot camera recordings with log files and time-series charts — all playing in real-time together
• Overhauled app performance as first accomplishment: resolved React re-rendering issues, implemented Redux + Reselect for proper state management. Became the de facto frontend lead by expertise
• Left when company secured a US Department of Defense contract (couldn't hire foreign workers). Founder recommended me directly to Streamlit's co-founder

Stack: React (class components), Redux, Re-Reselect, Node.js, Webpack, Plottable, Jest, Enzyme.
```
(~750 chars)

**Skills (5):** React.js, Redux, JavaScript, Node.js, UX Design

---

## 7. EXPERIENCE — EDIT OLX

**Current description:** Just a tech list ("Currently developing a global project working side by side with product & ux using the latest technologies: - ES6 - ReactJS...")

**New description:**
```
Almost 5 years at one of the world's largest classifieds platforms (Naspers/Prosus — 10,000+ employees, 317M monthly users, 30+ countries).

• Built ToOLX from scratch — a modular MVC framework that became the company's internal tools platform. Open-sourced on OLX's GitHub org. Modules: Category Tree, SEO Metatags, Translation Tool, Campaign URL Shortening, and more
• Grew from Argentina local market → international team (React/Redux/Node) → proposed relocation to Naspers Berlin office
• Developed global projects side by side with product & UX teams using React, Redux, Node.js, Express, Webpack
• Created imageCompressor — client-side image compression for the eCommerce platform

Stack evolved over 5 years: PHP/Symfony → AngularJS/Backbone → React/Redux/Node.js/Express.
```
(~780 chars)

**Skills (5):** React.js, JavaScript, Node.js, PHP, Redux

---

## 8. EXPERIENCE — EDIT NASPERS

**Current description:** "Working on a Global team developing a global dashboard in which you can create push notifications, check insights, define on which users are going to be sent."

**New description:**
```
Secondment from OLX to Naspers Berlin global competence center — Customer Lifecycle Management (CLM) team.

Built a global dashboard for push notifications, user insights, and targeting. The CLM system handled behavioral data of 300M monthly users worldwide, executing hundreds of millions of automated, personalized customer interactions across marketing and product channels.
```
(~370 chars)

**Skills (5):** JavaScript, React.js, Full-Stack Development, Software Design, UX Design

---

## 9. EXPERIENCE — EDIT FANSWORLD.TV

**Current:** Just a tech list (Symfony2, Doctrine, Twig, JSViews, HTML5, CSS3, jQuery, Meteor, Less)

**New description:**
```
First leadership role — led frontend development at the first online TV channel in Hispanic America (live streaming + on-demand, social television). Full-stack despite the frontend title: 35+ tracked issues spanning backend API work, frontend features, performance optimization, and email systems.

Built search optimization, profile sections, Isotope grid layouts, endless scroll, and Facebook API integration. Symfony2/PHP backend + jQuery/JSViews frontend.
```
(~430 chars)

**Skills (5):** JavaScript, jQuery, PHP, Symfony, CSS

---

## 10. EARLIER ROLES (DODICI, Altodot, Livra)

Keep as-is — these are old enough that minimal descriptions are fine per best practices. Optionally add 5 skills to each:

**DODICI:** PHP, Symfony, Linux, RFID, JavaScript
**Altodot:** PHP, JavaScript, jQuery, Facebook API, CSS
**Livra:** PHP, MySQL, PostgreSQL, Python, Linux

---

## 11. SKILLS SECTION

### Current top skills (by endorsements):
1. JavaScript — 23 endorsements
2. jQuery — 17 endorsements
3. PHP — 14 endorsements
4. MySQL — 12 endorsements
5. CSS — 10 endorsements

### Recommended top 3 to PIN:
1. **TypeScript** (currently buried)
2. **React.js** (currently buried)
3. **Node.js** (may not even exist — needs to be added)

### Skills to ADD (if not already present):
- Tailwind CSS
- AI/ML (or Artificial Intelligence)
- Amazon Web Services (AWS)
- Prisma
- Vite
- System Design
- Technical Leadership
- PostgreSQL (check if exists)
- Python (check if exists)
- Go
- Kubernetes

### Skills to DEPRIORITIZE (can't remove endorsements, but unpin):
- PHP, jQuery, Less, Bootstrap, Kohana Framework, XHTML, RequireJS, AJAX

---

## 12. OTHER SECTIONS

### Projects
- **Fansworld** — "Dec 2012 - Present" — should be updated to have an end date (not "Present")

### Featured Section (currently empty)
- Defer until personal website is built (Phase 3 of the overall plan)
- Could add: ToOLX docs link, 30DaysOfStreamlit Spanish repo

### Banner Image
- Defer — can create one later (Canva or custom)

### Open to Work
- Currently set to "Software Engineer roles"
- Recommend: switch to Recruiters-Only mode, add specific titles: "Senior Software Engineer", "Senior Product Engineer", "Staff Engineer", "Senior Frontend Engineer", "Engineering Manager"
- Locations: "Remote" + "Argentina" + "United States"

---

## Execution Order (via Chrome)

1. **Headline** — edit from profile header
2. **About** — edit from about section
3. **Add Mailberry** — click "+" on experience, fill all fields
4. **Edit Snowflake** — click pencil, add description + skills
5. **Edit Streamlit** — click pencil, replace description + add skills
6. **Edit Raven[Ops]** — click pencil, replace description + add skills
7. **Edit OLX** — click pencil, replace description + add skills
8. **Edit Naspers** — click pencil, replace description + add skills
9. **Edit FansWorld** — click pencil, replace description + add skills
10. **Add skills to DODICI, Altodot, Livra** — click pencil, add 5 skills each
11. **Skills section** — pin top 3, add missing skills
12. **Fix Fansworld project** — update end date
13. **Open to Work settings** — update titles, locations, mode

Each step requires your explicit confirmation before I execute it. I'll set "Notify network" to OFF for all changes to avoid spamming your connections.

---

## Verification
After all changes:
- Screenshot full profile
- Read profile text via Chrome to confirm everything saved
- Check headline in search preview (first 40-50 chars)
- Verify About section hook before the fold
- Confirm Mailberry shows as current role at the top
- Confirm Snowflake has a description
- Check pinned skills are TypeScript, React.js, Node.js
