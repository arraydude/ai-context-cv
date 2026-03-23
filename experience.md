# Experience

## 1. Mailberry — Senior Product Engineer (Founding Engineer)

- **Dates:** Apr 2025 - Present (~1 year)
- **Location:** Remote (company based in Los Angeles)
- **Company:** AI-native email service provider (ESP) for eCommerce. Replacement for Mailchimp/Klaviyo. Flagship product: "The Email Brain" — AI-powered system that automates email marketing strategy, content, and optimization.
- **Team size:** ~6 people (Founder/CEO, CTO, Head of Growth, Growth Advisor, Senior Platform Engineer, Senior Product Engineer)
- **How I got here:** After leaving Snowflake, wanted to learn new technologies and build something new. Daniel Nuske (CTO) — a long-time friend and colleague who has intersected multiple times across the career: Livra.com (early days), connected me with Randy at Raven[Ops], briefly worked together at Streamlit, and now Mailberry. Daniel proposed me as founding engineer, responsible for improving UI/UX and performance.

### What I did on day one — rebuilt the foundation

- **Multi-repo → monorepo migration** — consolidated the scattered codebase into a single monorepo architecture
- **Mantine → shadcn migration** — replaced the UI library with a more composable, customizable system
- **Next.js → Vite migration** — moved from outdated Next.js to Vite for a plain client-side app (no SSR needed)
- **Created the Design System package** — built from scratch on top of Tailwind + shadcn + Lucide, consumed by all frontend apps (autopilot, manager-portal)
- **TypeScript strictness overhaul** — improved type safety across the codebase, implemented proper ESLint + TSLint configuration to enforce good practices and block substandard code from merging
- **CI/CD safety checks** — added GitHub Actions checks on PRs preventing unwanted code from being merged
- **Telemetry implementation** — integrated PostHog for product analytics

### Email Text Editor (flagship frontend component)

- Built a **production-ready TipTap-based email template editor** optimized for react-email components
- **67 TypeScript/TSX files**, 18 TipTap base extensions, 7 React Email node types (Button, Divider, Heading, Image, Paragraph, BulletList, ListItem)
- Custom modal system (5 modal types with a consistent 4-component pattern), click-to-edit node configuration with real-time preview
- Advanced node position detection system for nested vs top-level elements
- Width management system (auto, full-width, percentage-based), padding extension with 8 granular commands, border system, alignment system
- 7 reusable shared field components, composable Zod validation schemas
- Email-optimized: all output uses @react-email/components for maximum email client compatibility
- Spec: `packages/design-system/.claude/TEXT_EDITOR_SPEC.md`

### AI-assisted development leadership

- As the product is AI-oriented, pushed to leverage AI for DX across the team
- Created Claude Code skills, agents, and commands for the Mailberry monorepo (see ai-workflows.md)
- Established standardized AI-assisted development workflows for the engineering team

### Ongoing work

- Building email automation flows (Autopilot) with AI-powered content generation
- Tailwind v3 → v4 migration across entire monorepo
- ESLint legacy → flat config (v8 → v9) migration
- npm → pnpm package manager migration
- Continuous Design System evolution (replacing custom components with shadcn, cross-package UI consistency)

### Technologies

- **Frontend:** React 18 + React Compiler, TypeScript, Vite 8, Tailwind v4, XState (state machines), shadcn/ui, TipTap (rich text editor), React Hook Form, Tanstack Query, React Router, PostHog, react-scan (performance monitoring)
- **Backend:** Node.js, Express, TypeScript, Prisma (ORM), PostgreSQL, DynamoDB, AWS (Lambda, S3, SQS, EventBridge, CloudFront, Serverless Framework)
- **AI:** Vercel AI SDK integrating Anthropic (Claude), OpenAI, Google GenAI, OpenRouter
- **Other:** Stripe (payments), SendGrid (email delivery), React Email (template rendering), Puppeteer/Crawlee (scraping), Slack integrations, Notion API

---

## 2. Snowflake — Software Engineer

- **Dates:** May 2022 - Apr 2025 (3 years)
- **Location:** Remote
- **Type:** Full-time

### Journey

1. Joined via **Streamlit acquisition** (Snowflake acquired Streamlit)
2. Worked on **Streamlit-in-Snowflake** — integrating Streamlit into the Snowflake ecosystem
3. Expanded to **main Snowflake web client** — touching multiple parts of the platform

### Technologies

- 

### Key achievements

- 
- 

> **STATUS: INCOMPLETE** — Awaiting detailed input from Nahuel about specific teams, products, technologies, and achievements at Snowflake.

---

## 3. Streamlit — Software Engineer

- **Dates:** Aug 2019 - May 2022 (2 years 10 months)
- **Location:** Remote from Argentina → San Francisco Bay Area startup
- **Company:** Open-source framework that lets data scientists build web apps from Python scripts. Founded 2018 by ex-Google X / Zoox engineers (Adrien Treuille, Thiago Teixeira, Amanda Kelly). Raised **$62M** from Sequoia Capital, Gradient Ventures, GGV Capital. **Acquired by Snowflake for ~$800M** (March 2022). 8M+ downloads, 1.5M+ apps built, 12K+ GitHub stars.
- **How I got here:** Recommended directly by Randy Shults (Raven[Ops] founder) to co-founder Thiago Teixeira
- **Early engineer** — joined when there was no cloud platform yet

### Growth arc

1. **Open-source framework** — Started contributing to the core Streamlit framework (Python + React)
2. **Cloud Platform frontend — built from scratch** — When the company decided to build a cloud platform for one-click app deployment, a small team was formed and I built the entire cloud platform frontend from the ground up
3. **Team growth** — As the platform grew, more frontend and backend engineers joined. Saw the company scale from a small team to acquisition

### Key achievement: Cloud Platform communication architecture

- Designed and implemented the **communication mechanism between Kubernetes → Streamlit hosted apps → iframe on Cloud Platform → PostMessage and WebSocket communication**
- Strongly typed end-to-end
- This was the critical bridge that made the cloud platform work — hosting user-created Streamlit apps inside the platform via iframes while maintaining real-time bidirectional communication

### Community contribution

- **Translated #30DaysOfStreamlit to Spanish** — self-proposed initiative to expand Streamlit's reach in the Spanish-speaking community during internal discussions about improving community engagement
- GitHub: `arraydude/30days-spanish`

### The journey

- Experienced the full startup arc: tiny team → open-source community growth → cloud platform launch → watching hosted apps grow → **$800M acquisition by Snowflake**
- Strong team culture — "ponerse la camiseta" (giving everything for the team)

### Technologies

- **Frontend (Cloud Platform):** TypeScript, ReactJS, SWR, HTML, SCSS, TailwindCSS
- **Framework:** Python 2/3, Go
- **Infrastructure:** Kubernetes (learned on the job), WebSockets, PostMessage API, iframes
- **Testing:** Jest, Cypress
- **Collaboration:** UX/UI design

---

## 4. Raven[Ops] — Full Stack Engineer

- **Dates:** Dec 2018 - Aug 2019 (9 months)
- **Location:** Remote from Argentina → San Francisco Bay Area startup
- **Company:** "DevOps for robotics" — tools to collect, stream, visualize, and manage robot data. Founded 2015, funded by **Accel** ($3.5M). Team: 3 founders, 5 devs, 1 PO, 1 sales manager.
- **First remote job for the US market** — entry point into the SF/US tech ecosystem

### What I did

- Built an intuitive **web interface to visualize datasets for robotics**
- The tool allowed the QA team to **visualize and tag data** to iterate AI models faster
- Key feature: view dataset **video recordings from robot cameras** alongside log files and **time-series data charts** that played in sync with the video
- Detected key events and extracted data across perception, time-series, and log file fields

### Key achievement

- **Performance overhaul** — First accomplishment was improving the entire app's performance. Resolved re-rendering issues, implemented Redux and Reselect for proper state management. This was the React class components era, and no one else on the team had experience with React/Redux at the time. Became the frontend lead by expertise.

### How it ended

- Company secured a contract with the **US Department of Defense**, which meant they couldn't hire foreign workers. Founder **Randy Shults recommended me to Thiago Teixeira** (co-founder of Streamlit), directly leading to the next role. The company later shut down.

### Technologies

- HTML5, CSS3
- JavaScript/ES6, Node.js
- ReactJS (class components), Redux, Re-Reselect
- Webpack, Babel
- Plottable (charting)
- Jest, Enzyme
- UX/UI

---

## 5. OLX — Fullstack Software Engineer

- **Dates:** Mar 2014 - Nov 2018 (4 years 9 months)
- **Location:** Buenos Aires, Argentina → Berlin, Germany
- **Company:** Global online classifieds marketplace (owned by Naspers/Prosus). 10,000+ employees, 317M monthly users, 20+ brands across 30+ countries, ~$2.9B revenue.

### Growth Arc

1. **Argentina market** — Started working on local classifieds platform
2. **Built ToOLX** — Created a modular MVC framework from scratch (`s2r2Framework` engine) that became the company's internal tools platform. This is what made me notable within the company.
3. **International team** — Moved to global platform development, working side by side with product & UX using modern frontend stack (React, Redux, ES6)
4. **Berlin / Naspers** — Team was proposed to relocate to Naspers Berlin office (CLM team)

### ToOLX (signature project)

- **Modular MVC framework built from scratch** for managing organizational processes across OLX
- Open-sourced on OLX's GitHub org (`olx-inc/toolx`), engine extracted as `s2r2Framework`
- Built-in modules: Category Tree Manager, Keywords Report of Ads, Deploy SEO Metatags, Translation Tool, Expiration Rules, Item Rebump, Campaign URL Shortening
- Features: ACL (role-based access control), JIRA integration, automated module generation toolkit, session management, batch processing with crons, AJAX controllers, CSV/JSON rendering
- Architecture: PHP + Twig templating + MySQL + Apache, YAML configuration, modular routing (module/controller/action)
- Designed for simplicity and scalability — teams could spin up new functional modules quickly

### imageCompressor

- Client-side image compression module to improve image uploading for OLX's eCommerce platform

### Technologies

- **Modern stack (international team):** ES6, ReactJS, Redux, NodeJS, Express, Webpack, Sass, Karma
- **Earlier stack (Argentina):** AngularJS, Backbone, Underscore, Grunt, Bower, RequireJS
- **ToOLX/Backend:** PHP5, Twig, Doctrine, Composer, MySQL, MariaDB, MongoDB
- **Other:** Socket.IO, Gulp, Agile methodology

### 5b. Naspers — Software Engineer (CLM Team, Berlin)

- **Dates:** May 2016 - Aug 2016 (4 months)
- **Location:** Berlin, Germany (Naspers global competence center)
- **Team:** Customer Lifecycle Management (CLM) — ~30 people at the Berlin center
- Built a **global dashboard** for push notifications, insights, and user targeting
- CLM handled behavioral data of **300M monthly users worldwide**, executing hundreds of millions of targeted, automated, personalized customer interactions across marketing and product channels

---

## 6. FansWorld TV — Frontend Leader

- **Dates:** ~2012 - 2013
- **Location:** Buenos Aires, Argentina
- **Company:** First online TV channel in Hispanic America — live streaming + on-demand, designed exclusively for the internet. Started as a social network for sports fans (2011), pivoted to social television (2013). Users could interact in real-time with content. Own building in Buenos Aires, iOS/Android apps.
- **First leadership role**

### What I did
- Led frontend development for the social network / streaming platform
- Worked **full-stack** despite the frontend title — 35 tracked issues spanning backend API work, frontend features, performance optimization, and email systems
- Backend: refactored controllers, serialization, API bug fixes, search performance optimization, profile sections, filter systems
- Frontend: implemented Isotope grid layouts, endless scroll, toolbar redesign, loading states, video tabs, highlight lists
- Built welcome email system (view + backend), notification email cleanup
- Facebook API integration for social features

### Technologies

- **Backend:** PHP / Symfony2, Twig templating
- **Frontend:** JSViews, HTML5, CSS3, jQuery, Less, SVG, Isotope
- **APIs:** Facebook API
- **Repo:** `FansWorldTV/web` — 4.6M lines PHP, 1.7M lines JS, 645K lines CSS

---

## 7. DODICI Corporation — Software Developer

- **Dates:** ~2011 - 2012
- **Location:** Buenos Aires, Argentina

### What I did
- Software development with PHP/Symfony2 stack
- Worked on RFID (radio-frequency identification) integration projects
- Linux server administration

### Technologies

- PHP, Symfony2, Doctrine
- Radio-frequency identification (RFID)
- Linux, CSS, HTML
- Facebook API

---

## 8. Altodot / The Fan Machine — Software Developer

- **Dates:** Oct 2010 - Aug 2011 (10 months)
- **Location:** Buenos Aires, Argentina

### Technologies

- PHP5, Symfony
- JavaScript, jQuery
- HTML, CSS
- Facebook API, Twitter API

---

## 9. Livra.com — PHP Developer & IT Operations

- **Dates:** Jan 2009 - Oct 2010 (1 year 9 months)
- **Location:** Buenos Aires, Argentina

### Technologies

- PHP5, Python
- MySQL, PostgreSQL
- Linux
- JavaScript

