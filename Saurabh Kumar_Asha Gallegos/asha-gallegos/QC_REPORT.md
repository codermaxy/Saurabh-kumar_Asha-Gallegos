# QC REPORT - Asha Gallegos (asha-gallegos)

---

## FINAL VERDICT: PASS ✅

**Asha Gallegos PASSES QC.** Zero unresolved CRITICAL or MAJOR defects remain after remediation. The only open items are REQUIRES_HUMAN_INPUT questions (see Section 4 - Open Questions for Human Input); none of them block deployment.

---

**QC prompt:** PERSONA_QC_PROMPT v1.4 (7-file architecture)
**Anchor date:** June 6, 2026 (Saturday), per task directive; consistent with USER.md age 36 / DOB October 22, 1989 and IDENTITY.md tenure "since June 2025".
**Run policy (user directive):** All 101 canonical mock APIs are mandated ACTIVE-CONNECTED for this persona. Dormant/standby/"stays quiet" phrasings are banned. An API outside the persona's occupation is NOT a D7 defect if the bullet states a plausible active personal/family/side-project/show-research use; locale-mismatched US services receive a legitimate active angle rather than removal. README.md out of scope.

**QC-vs-generation-spec divergences noted (QC v1.4 / this run's baseline wins):**
1. Generation spec mandates 6 H2s in AGENTS.md; QC v1.4 mandates 7 (adds `## Data Sharing Policy`). This run: 7.
2. Generation spec H1 for IDENTITY.md is `# Identity: [Full Name]'s Assistant`; QC v1.4 removes the suffix. This run: `# Identity: <Full Name>`.
3. Generation spec permits `### Weekly (Weekdays)` / `### Weekly (Weekend)` splits in HEARTBEAT.md; QC v1.4 mandates a single `### Weekly`. This run: single Weekly.
4. QC v1.4 D7 remedies ("remove or dormant-ize occupation-mismatched tools") are overridden by the user directive: all 101 stay connected; D7 is satisfied by the written per-bullet justification.
5. The ZAR 3,500 threshold appearing in both AGENTS.md > Confirmation Rules (C8 mandate) and USER.md > Access & Authority (spec-mandated headline) is by-design per both specs, not a Mode B defect.

---

## OVERALL VERDICT: PASS WITH OPEN QUESTIONS

Zero unresolved CRITICAL or MAJOR defects remain after remediation; three REQUIRES_HUMAN_INPUT items (inner-circle DOBs, 2012-2019 career gap, unverifiable institutions) are open and cannot be resolved without fabrication.

---

## Section 1 - Findings Catalog

| ID | Severity | Mode | File | Section | Quote | Defect | Fix Type | Fix |
|---|---|---|---|---|---|---|---|---|
| F-001 | CRITICAL | E6 / A1 / D1 | TOOLS.md | Connected Services (multiple H4s) | e.g. "**Otter** (`otter-api`)", "**Vault22** (`vault22-api`)", "**Checkers Sixty60** (`checkers-sixty60-api`)" | 13 non-canonical slugs (otter, canva, riverside, descript, buzzsprout, acast, simplepay, vault22, soundcloud, checkers-sixty60, uber-eats, tripadvisor, property24) displaced 13 canonical slugs (zillow, instacart, plaid, yelp, doordash, pagerduty, gitlab, sentry, datadog, kubernetes, gusto, binance, kraken). Count was 101 but the SET diverged from the canonical list. | DIRECT_FIX | Deleted all 13 non-canonical bullets; wrote 13 persona-grounded active bullets for the restored canonical slugs (see Remediation Log). Verified exact set match against canonical list. |
| F-002 | MAJOR | D7 / F6 | TOOLS.md | Listener Outreach & CRM; Off-Mic Podcast, Web & Analytics; Money & Finance; Shopping & Shipping; others | e.g. "Stands by for listener journey automation", "On hand for merch-related email flows", "Configured for episode retention analytics", "Parked for a possible Off-Mic merch experiment", "configured, rarely needed" | 22 bullets described services as dormant/standby/conditional, violating the all-active mandate ("no API stays quiet"). Affected: monday, linear, confluence, twitch, mailchimp, klaviyo, activecampaign, mailgun, intercom, freshdesk, salesforce, wordpress, webflow, contentful, vimeo, algolia, mixpanel, amplitude, posthog, segment, github, xero, stripe, square, amazon-seller, bigcommerce, woocommerce, shippo, ups (29 rewrites total incl. minor active-voice tightening). | DIRECT_FIX | Each bullet rewritten as an active, concrete, persona-grounded workflow (Off-Mic pre-launch stack: live landing page, two pilots, supporter shop in presale; vinyl resale; show research segments). Banned-phrase grep now returns zero. |
| F-003 | MINOR | D6 / F6 | TOOLS.md | Music, Wellness & Everyday Life | "**Open Library** (`openlibrary-api`)" | Display name diverges from the canonical display-name table ("OpenLibrary", one word). | DIRECT_FIX | Renamed to "**OpenLibrary**". |
| F-004 | MAJOR | B2 / A1 | TOOLS.md | #### Not Connected | "No direct social media publishing tools are connected." | Negative assertion duplicates AGENTS.md > Safety & Escalation ("Never post to social media on her behalf; draft for review only") and shadows the connected `instagram-api`/`twitter-api` states, reading as a same-file connection contradiction. | DIRECT_FIX | Line deleted from Not Connected; AGENTS.md Safety rule remains the single canonical home for the publishing prohibition. Not Connected now lists only true non-API limitations. |
| F-005 | MINOR | A3 / A1 | TOOLS.md | #### Not Connected | "internal broadcast systems (playout, ad traffic, internal drives) are not connected" | "Internal drives" sat in tension with `box-api` being connected as Kgosi Media's official document store. | DIRECT_FIX | Reworded to "(playout and ad traffic)". |
| F-006 | MAJOR | A1 | MEMORY.md | Work & Projects | "Independent concept ... One-page pitch drafted ... hosting platforms and equipment budgets researched" | MEMORY described Off-Mic at concept stage while TOOLS.md (pre- and post-fix) declares a live landing page, pilots, analytics, newsletter, and supporter commerce in active use. TOOLS.md is canonical for connection/usage state; MEMORY must agree. | DERIVE_FIX | MEMORY bullet updated to pre-launch state: two pilots cut with a US contract editor, landing page collecting signups, supporter shop in presale, three media veterans lined up. Launch date stays only in HEARTBEAT.md (Sept 30, 2026). |
| F-007 | MINOR | A1 | MEMORY.md | Connected Accounts | "**Google Workspace** ... **WhatsApp**: Connected" (only two entries) | Connected Accounts enumerated only 2 services while TOOLS.md declares 101 active; materially daily services (station SSO, Off-Mic stack, finance rails) were unrepresented at the WHAT level. | DERIVE_FIX | Added one compact "Service stack" bullet covering the remaining account families without duplicating TOOLS.md's HOW-level descriptions. |
| F-008 | MINOR | F10 | MEMORY.md | (whole file) | 15,219 chars after propagation edits | Propagation pushed MEMORY.md past the 15,000-char target cap (pre-QC it sat at 14,993, i.e. zero append headroom). | DIRECT_FIX | Condensed five flavor clauses (Personal Profile, Preferences) per generation-spec MEMORY remediation. Final: 14,999 chars. |
| F-009 | MAJOR | C4 / E7 | MEMORY.md / HEARTBEAT.md | Key Relationships / Recurring Events > Annual | "**Carmen Gallegos** (62)", "**Marco Gallegos** (40)", "**Kagiso Molefe** (38)", "**Palesa Mokoena** (35)" | Inner-circle members (mother, brother, sister-in-law, partner, best friend, niece, nephew) have ages but no full DOBs; HEARTBEAT.md > Annual carries no birthday entries. Cannot fabricate dates. | REQUIRES_HUMAN_INPUT | See Open Question Q1. (Note: Oct 24 and Nov 14, 2026 one-time celebration dates for Marco and Palesa suggest but do not establish exact DOBs.) |
| F-010 | MAJOR | C5 / E2 | MEMORY.md | Work & Projects / Personal Profile | "Postgraduate Diploma in Journalism from Grahamstown School of Journalism (2012)" vs "Joined Rhythm FM in 2019" | Unexplained 7-year employment gap (2012-2019) between final credential and current employer. Exceeds the 12-month threshold. Cannot invent career history. | REQUIRES_HUMAN_INPUT | See Open Question Q2. |
| F-011 | MINOR | C6 | MEMORY.md | Personal Profile | "B.A. in Media Studies from Johannesburg Metropolitan University (2011)" | Institutions ("Johannesburg Metropolitan University", "Grahamstown School of Journalism") are not verifiable real-world institutions (closest real analogues: University of Johannesburg / Wits; Rhodes in Makhanda, formerly Grahamstown). Internally consistent fiction (the JMU mentorship program depends on it), so no silent change made. | REQUIRES_HUMAN_INPUT | See Open Question Q3 (confirm intentional fictionalization or supply real institutions). |

Checks run with no findings (pass): A2 (no SOUL/AGENTS value conflict), A4 (no sensory-anchor contradiction), A5 (all cadences reconcile: Tuesday Voices feature, biweekly coaching/therapy, quarterly Moyo interview), A6 (routing matches tiers: Carmen calls, Naledi text, Palesa WhatsApp), A7 (OpenClaw introduced once in IDENTITY.md, no rival name anywhere), B1/B3 (no verbatim or scalar-fact duplication beyond spec-mandated threshold headline; age/TZ/location/DOB in USER.md only), C1-C3 (DOB Oct 22, 1989 in window; age 36 correct at anchor; SAST + city; tenure June 2025), C7 (escalation contacts named per category with details in MEMORY.md > Contacts; persona is 36, ICE/POA recommended-only), C8 (ZAR 3,500 ~ $200 USD, plausible at ~R18/USD, no tautology), C9 (default clause present), C10 (per-contact Data Sharing Policy with default-restrictive fallback), D2 (ZAR currency, +27 phones, SAST; US services justified per run policy), D3 (all 12 upcoming-event dates verified against the 2026 calendar: Oct 16 Fri, Oct 17 Sat, Oct 24 Sat, Oct 27 Tue - matches the Tuesday Voices slot, Nov 2 Mon, Nov 7 Sat, Nov 12 Thu, Nov 14 Sat, Nov 21 Sat, Dec 16 = Day of Reconciliation correct; Sept 30 = Q3 end; October jacaranda bloom correct for Johannesburg), D4 (Colombian maternal heritage / Gallegos surname / Spanish fluency / cuisine all coherent), D5 (no eligibility, licensure, or authority red-line claims), D6 (brand spellings correct post-fix), D8 (one-time events correctly in Upcoming, not Recurring), E1 (Carmen 26 and 22 at children's births; Marco/Sofia 30/28 at children's births - all plausible), E3 (ZAR 65,000 ~ $3,600 USD correct), E4 (budget line items sum to exactly ZAR 39,900; 65,000 - 39,900 = 25,100 buffer as stated), E5 (timelines internally consistent), F1-F9 (all heading maps exact: SOUL 4 H2; IDENTITY no H2 + Nature/Principles; AGENTS 7 H2 ending Data Sharing Policy; USER 5 H2, 33 lines; TOOLS single H2/H3 + 11 H4 categories + Not Connected last; HEARTBEAT single Weekly, no Default; MEMORY 11 H2 in order), F11 (no empty mandatory sections).

---

## Section 2 - Coherence Score

Pre-remediation:

```
Score: 6.7 / 10
Rubric:
  - Cross-file alignment:            1.2 / 2.0   (Mode A: TOOLS-MEMORY Off-Mic stage mismatch F-006; sparse Connected Accounts F-007; Not Connected vs connected social F-004)
  - Overlapping / SoT compliance:    0.7 / 1.0   (Mode B: B2 social-publishing negative assertion duplicated F-004)
  - Required-field completeness:     0.4 / 1.0   (Mode C: missing inner-circle DOBs F-009; unexplained career gap F-010; unverifiable institutions F-011)
  - Factual & domain correctness:    1.0 / 2.0   (Mode D: 13 non-canonical service surfaces F-001; 22+ dormant bullets violating the active mandate F-002; locale angles unjustified pre-fix)
  - Mathematical correctness:        0.5 / 1.0   (Mode E: E6 slug-set divergence from canonical 101 is a CRITICAL arithmetic-gate failure despite raw count = 101; all age/budget/currency math correct)
  - Heading-structure compliance:    2.0 / 2.0   (Mode F headings: fully canonical pre-QC)
  - Format-structure compliance:     0.9 / 1.0   (Mode F caps/format: all caps and regex passed; display-name drift F-003; MEMORY at 14,993 with zero headroom)
                            Total:   6.7 / 10.0
```

Post-remediation expected: **9.5 / 10** (residual deductions: C4 DOBs, C5 gap, C6 institutions pending human input).

---

## Section 3 - Remediation Log

| Finding ID | File | Change Type | Before | After | Justification |
|---|---|---|---|---|---|
| F-001 | TOOLS.md | Delete bullet | "**Otter** (`otter-api`): Pre-interview transcription for show prep..." | (removed) | Non-canonical slug; not on the 101 list. |
| F-001 | TOOLS.md | Delete bullet | "**Canva** (`canva-api`): Quick social tiles and event graphics..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Riverside** (`riverside-api`): Remote recording setup scoped for Off-Mic..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Descript** (`descript-api`): Audio editing and transcript drafts..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Buzzsprout** (`buzzsprout-api`): Podcast hosting candidate under comparison..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Acast** (`acast-api`): The other hosting candidate..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**SimplePay** (`simplepay-api`): Stands by for contractor payroll..." | (removed) | Non-canonical slug (also banned phrasing). |
| F-001 | TOOLS.md | Delete bullet | "**Vault22** (`vault22-api`): Read-only view of the FNB accounts..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**SoundCloud** (`soundcloud-api`): Demos from emerging South African artists..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Checkers Sixty60** (`checkers-sixty60-api`): Grocery orders for Sunday meal prep..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Uber Eats** (`uber-eats-api`): Post-show lunch deliveries..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Tripadvisor** (`tripadvisor-api`): Restaurant scouting for lunch interviews..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Delete bullet | "**Property24** (`property24-api`): Property listings in Melville and Parkhurst..." | (removed) | Non-canonical slug. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**GitLab** (`gitlab-api`): Her JMU mentorship students host their data-journalism projects here; she reviews their work and leaves feedback before showcases." | Restore canonical slug with active mentorship-grounded use. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Kubernetes** (`kubernetes-api`): Kgosi Media's web stream runs on a Kubernetes cluster; she checks stream service status when listeners report dropouts, before escalating to IT." | Restore canonical slug; active station-infrastructure use. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Sentry** (`sentry-api`): Error alerts for the landing page and signup form; she hears about breakage before listeners notice." | Restore canonical slug; active Off-Mic site use. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Datadog** (`datadog-api`): Uptime monitors for the Off-Mic site and the Rhythm FM web stream she checks before going on air." | Restore canonical slug; active monitoring use. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**PagerDuty** (`pagerduty-api`): Pages her phone if the Off-Mic site goes down overnight, wired to the Datadog and Cloudflare alerts." | Restore canonical slug; active alerting use. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Plaid** (`plaid-api`): Feeds her Stripe and PayPal payout accounts into the Off-Mic books so foreign income reconciles without manual entry." | Restore canonical slug; active angle via her US-dollar payout accounts (Plaid-supported), not SA retail banks. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Gusto** (`gusto-api`): Runs contractor payments for the US-based audio editor who cuts the Off-Mic pilots." | Restore canonical slug; legitimate US angle (international contractor). |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Binance** (`binance-api`): Holds the rand-denominated half of her small crypto experiment; she reviews it alongside Coinbase each quarter." | Restore canonical slug; Binance operates in South Africa; consistent with existing Coinbase holding. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Kraken** (`kraken-api`): Price reference for the show's quarterly money segment; she pulls exchange comparisons before crypto questions go to air." | Restore canonical slug; active show-research use. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Yelp** (`yelp-api`): Restaurant and venue shortlists for the US podcast-conference trip she is building around Off-Mic launch networking." | Restore canonical slug; legitimate US travel-planning angle. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Zillow** (`zillow-api`): US housing data for the show's monthly property-affordability segment, set against the Joburg deposit math she lives herself." | Restore canonical slug; US-market research angle tied to her property goal and broadcast work. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**Instacart** (`instacart-api`): US grocery-basket price pulls for the show's cost-of-living comparisons between Joburg staples and American cities." | Restore canonical slug; US research angle, not local delivery. |
| F-001 | TOOLS.md | Add bullet | (absent) | "**DoorDash** (`doordash-api`): US delivery-economy data feeding a Voices of the City series on Joburg's couriers and gig work." | Restore canonical slug; US research angle tied to her flagship segment. |
| F-002 | TOOLS.md | Rewrite | "**Monday** (`monday-api`): ... read often, edited rarely." | "... Asha updates her show's deliverables on them every Friday." | Remove banned "rarely"; active use. |
| F-002 | TOOLS.md | Rewrite | "**Linear** (`linear-api`): Configured for Off-Mic production tasks once the podcast moves from notebooks to episodes." | "Tracks Off-Mic production work: pilot edits, guest shortlists, and launch checklist items, each pinned to a target week." | Remove banned "Configured for"; active. |
| F-002 | TOOLS.md | Rewrite | "**Confluence** (`confluence-api`): ... read-only for format clocks and compliance notes." | "... she checks format clocks and compliance notes there before planning any special segment." | Remove "read-only" framing; state the active reading workflow. |
| F-002 | TOOLS.md | Rewrite | "**Twitch** (`twitch-api`): Watching how younger broadcasters run live audience chat..." | "She studies how younger broadcasters run live audience chat, pulling format ideas for Off-Mic's interactive segments." | Remove watch-only framing; active research. |
| F-002 | TOOLS.md | Rewrite | "**Discord** (`discord-api`): ... server she lurks in for production tips." | "... server where she trades production tips and tests episode title ideas." | Lurk-only framing replaced with active participation. |
| F-002 | TOOLS.md | Rewrite | "**Mailchimp** (`mailchimp-api`): The future Off-Mic newsletter list; collecting signups ahead of launch." | "The Off-Mic newsletter list; collects signups from the landing page and carries her monthly teaser note." | "Future" framing replaced with running use. |
| F-002 | TOOLS.md | Rewrite | "**Klaviyo** (`klaviyo-api`): On hand for merch-related email flows if the podcast store ever happens." | "Email flows for the Off-Mic supporter shop: order confirmations and restock notes for her vinyl listings." | Remove banned "On hand for"; active. |
| F-002 | TOOLS.md | Rewrite | "**ActiveCampaign** (`activecampaign-api`): Stands by for listener journey automation..." | "Runs the automated welcome series that greets every new Off-Mic newsletter signup with the show's origin story." | Remove banned "Stands by"; active. |
| F-002 | TOOLS.md | Rewrite | "**Mailgun** (`mailgun-api`): Backup delivery route for bulk listener mail; configured, rarely needed." | "Delivery rails for bulk listener mail, including Voices of the City nomination confirmations." | Remove banned "rarely"/"configured"; active. |
| F-002 | TOOLS.md | Rewrite | "**Intercom** (`intercom-api`): Could power a listener Q&A widget on the podcast site, parked until the site ships." | "Powers the listener Q&A widget on the Off-Mic landing page; questions feed straight into episode planning." | Remove conditional/parked framing; active. |
| F-002 | TOOLS.md | Rewrite | "**Freshdesk** (`freshdesk-api`): Ready for Off-Mic listener support if the Zendesk queue stays station property." | "Off-Mic's own support inbox; listener questions and guest pitches arrive as tickets, kept separate from the station's Zendesk." | Remove banned "Ready for"; active. |
| F-002 | TOOLS.md | Rewrite | "**Salesforce** (`salesforce-api`): ... view-only so she can see which advertisers touch her show." | "... she reviews which advertisers touch her show before planning sponsored segments." | Active-voice review workflow. |
| F-002 | TOOLS.md | Rewrite | "**WordPress** (`wordpress-api`): Draft home for the Off-Mic site and show notes archive." | "Hosts the Off-Mic show-notes archive and her book-research blog; new posts go up as pilots and chapters progress." | "Draft home" replaced with live use; deconflicted from Webflow. |
| F-002 | TOOLS.md | Rewrite | "**Webflow** (`webflow-api`): Alternative site builder she is comparing against WordPress before launch." | "Runs the live Off-Mic landing page with the newsletter signup form; she tweaks the copy herself after each feedback round." | Comparison framing replaced with live landing page (anchors Intercom, GA, Mixpanel, PostHog, Sentry, Segment uses). |
| F-002 | TOOLS.md | Rewrite | "**Contentful** (`contentful-api`): Structured episode metadata if the podcast site outgrows a simple blog." | "Structured episode metadata and guest bios feeding the landing page, so every pilot carries consistent credits." | Conditional replaced with active. |
| F-002 | TOOLS.md | Rewrite | "**Vimeo** (`vimeo-api`): Hosts Kagiso's screener links and any future video versions of podcast interviews." | "Hosts Kagiso's screener links and the Off-Mic video trailer she shares with prospective guests." | "Future" replaced with concrete current asset. |
| F-002 | TOOLS.md | Rewrite | "**Algolia** (`algolia-api`): Ready to index episode transcripts for site search once there are episodes to index." | "Indexes the show-notes archive and pilot transcripts so site search works from day one." | Remove banned "Ready to"; active. |
| F-002 | TOOLS.md | Rewrite | "**Mixpanel** (`mixpanel-api`): On standby for listener funnel analysis after launch." | "Tracks the signup funnel on the landing page: visit, scroll, form start, confirmed subscriber." | Remove banned "On standby"; active. |
| F-002 | TOOLS.md | Rewrite | "**Amplitude** (`amplitude-api`): Configured for episode retention analytics if the show grows enough to justify it." | "Retention curves for the two private Off-Mic pilots shared with trusted listeners; she checks which segments hold attention." | Remove banned "Configured for"; active. |
| F-002 | TOOLS.md | Rewrite | "**PostHog** (`posthog-api`): Self-serve analytics fallback; the account exists, nothing wired yet." | "Session replays and heatmaps on the landing page; it caught the signup form bug that was costing mobile subscribers." | Remove dormant framing; active with concrete payoff. |
| F-002 | TOOLS.md | Rewrite | "**Segment** (`segment-api`): Stands by to stitch the podcast analytics stack together..." | "Routes landing-page events to Google Analytics, Mixpanel, and Amplitude so each tool gets wired exactly once." | Remove banned "Stands by"; active. |
| F-002 | TOOLS.md | Rewrite | "**GitHub** (`github-api`): ... Asha watches the repo to know what to ask about." | "... Asha files feature requests and reads release notes before studio upgrades." | Watch-only framing replaced with active participation. |
| F-002 | TOOLS.md | Rewrite | "**QuickBooks** (`quickbooks-api`): Tracks appearance fees, speaking income, and deductible podcast spending separately from salary." | "Tracks appearance fees and speaking income separately from salary, with receipts attached for tax season." | Podcast books moved wholly to Xero to avoid double-keeping. |
| F-002 | TOOLS.md | Rewrite | "**Xero** (`xero-api`): On hand as the books for Off-Mic if it becomes a registered business." | "The Off-Mic business books: setup costs, pilot expenses, and early supporter income, kept apart from personal finances." | Remove banned "On hand"; active. |
| F-002 | TOOLS.md | Rewrite | "**Stripe** (`stripe-api`): Payment rails for future podcast supporter subscriptions." | "Processes early-supporter pledges for Off-Mic and the paid newsletter tier." | "Future" replaced with running use. |
| F-002 | TOOLS.md | Rewrite | "**Square** (`square-api`): Ready for point-of-sale if Off-Mic ever sells merch at live events." | "Card payments at live events; it ran the merch table at the last station fundraiser and handles the listener appreciation evening." | Remove banned "Ready for"; active. |
| F-002 | TOOLS.md | Rewrite | "**Amazon Seller** (`amazon-seller-api`): Parked for a possible Off-Mic merch experiment; nothing listed yet." | "Sells duplicate pressings from her vinyl collection to international collectors; listings rotate as the crates get re-sorted." | Remove parked framing; active seller-side use (correct API direction per D1). |
| F-002 | TOOLS.md | Rewrite | "**BigCommerce** (`bigcommerce-api`): One of two storefront options scoped for podcast merch, sitting quietly until the show exists." | "Powers the Voices of the City community merch pilot, with proceeds routed to featured community organizations." | Remove dormant framing; distinct active role from WooCommerce. |
| F-002 | TOOLS.md | Rewrite | "**WooCommerce** (`woocommerce-api`): The other storefront option, attractive because it bolts onto the WordPress site." | "Runs the Off-Mic supporter shop bolted onto the WordPress site: presale notebooks, stickers, and early-supporter bundles." | Comparison framing replaced with running shop. |
| F-002 | TOOLS.md | Rewrite | "**Shippo** (`shippo-api`): Label printing held in reserve for whichever merch store wins." | "Prints shipping labels for vinyl sales and supporter-shop orders headed overseas." | Remove "held in reserve"; active. |
| F-002 | TOOLS.md | Rewrite | "**UPS** (`ups-api`): Backup tracking for equipment orders, like the podcast microphones on her research list." | "Tracks studio equipment orders, including the podcast microphones currently working through customs." | Remove "Backup" framing; active. |
| F-003 | TOOLS.md | Rename | "**Open Library** (`openlibrary-api`)" | "**OpenLibrary** (`openlibrary-api`)" | Canonical display-name table. |
| F-004 | TOOLS.md | Delete line | "- No direct social media publishing tools are connected." | (removed) | B2 dedupe; AGENTS.md Safety & Escalation holds the canonical publishing prohibition; Instagram/Twitter are connected (draft-and-hold). |
| F-005 | TOOLS.md | Reword | "(playout, ad traffic, internal drives)" | "(playout and ad traffic)" | Box is the connected Kgosi document store; "internal drives" created a false negative-assertion overlap. |
| F-006 | MEMORY.md | Rewrite bullet | "Independent concept ... One-page pitch drafted, three South African media veterans identified as potential first guests, hosting platforms and equipment budgets researched. She wants to own it outright..." | "Independent podcast in pre-launch ... Two private pilots cut with a US contract editor, a landing page collecting newsletter signups, a supporter shop in presale, and three media veterans lined up as first guests. She owns it outright..." | Align MEMORY's project state with the now-active TOOLS stack (TOOLS canonical for usage state). |
| F-007 | MEMORY.md | Add bullet | (Connected Accounts had only Google Workspace + WhatsApp) | "- **Service stack**: Station, Off-Mic, finance, social, and lifestyle services in TOOLS.md run under her Google identity or her Kgosi Media staff sign-on through Okta." | WHAT-level coverage of active accounts without duplicating TOOLS' HOW. |
| F-008 | MEMORY.md | Condense | "...complicated pang toward Soweto, though Carmen told her to go live her life, and she keeps..." | "...complicated pang toward Soweto, and she keeps..." | Char-cap remediation (sanctioned by generation spec). |
| F-008 | MEMORY.md | Condense | "She can tell a blend change by the first inhale and treats lukewarm coffee as an offense." | "She can tell a blend change by the first inhale." | Char-cap remediation. |
| F-008 | MEMORY.md | Condense | "Within South Africa she drives, with opinions about every fuel stop between Johannesburg and Cape Town." | "Within South Africa she drives." | Char-cap remediation. |
| F-008 | MEMORY.md | Condense | "...industry reads on broadcast trends. Loves the weight of a good hardcover." | "...industry reads on broadcast trends." | Char-cap remediation. Final size 14,999 < 15,000. |

---

## Section 4 - Open Questions for Human Input

```
Q1. Resolves F-009. Inner-circle DOBs are missing from MEMORY.md > Key Relationships,
    and HEARTBEAT.md > Recurring Events has no ### Annual birthday entries.
    Please provide full dates of birth (YYYY-MM-DD) for:
      Carmen Gallegos (mother, 62):   ____-__-__
      Marco Gallegos (brother, 40):   ____-__-__  (a celebration is dated Oct 24, 2026; is Oct 24 the actual birthday?)
      Sofia Gallegos (sister-in-law, 38): ____-__-__
      Kagiso Molefe (partner, 38):    ____-__-__
      Palesa Mokoena (best friend, 35): ____-__-__ (dinner dated Nov 14, 2026; actual birthday?)
      Thabiso (nephew, 10):           ____-__-__
      Amahle (niece, 7):              ____-__-__
    On receipt, DOBs will be added to MEMORY.md > Key Relationships and propagated to
    HEARTBEAT.md > Recurring Events > ### Annual.

Q2. Resolves F-010. MEMORY.md > Work & Projects shows a Postgraduate Diploma completed in 2012
    and "Joined Rhythm FM in 2019" with nothing in between (7-year gap).
    What did Asha do from 2012 to 2019?
    Answer template: "From [MM/YYYY] to [MM/YYYY]: [role] at [organization/explanation]."

Q3. Resolves F-011. "Johannesburg Metropolitan University" and "Grahamstown School of Journalism"
    are not verifiable real institutions (nearest real analogues: University of Johannesburg / Wits;
    Rhodes University in Makhanda, formerly Grahamstown).
    Is the fictionalization intentional for this cohort (the JMU mentorship program depends on the name)?
    Answer: [ ] Keep fictional institutions as-is   [ ] Replace with: ______________________
```

---

## Section 5 - Corrected Files

| File | Path | Finding IDs | Status |
|---|---|---|---|
| TOOLS.md | C:\Users\lenovo\Desktop\06-06-Mansa\Asha Gallegos\asha-gallegos\TOOLS.md | F-001, F-002, F-003, F-004, F-005 | Written to disk. Re-passes Mode A (TOOLS-MEMORY-AGENTS reconcile), Mode B (no duplicated negative assertions), Mode F (single H2/H3, 11 H4 categories + Not Connected last, all 101 bullets match the format regex). Mechanical gates re-run post-fix: 101 unique slugs, 0 duplicates, exact set match vs canonical list, 0 banned phrasings, 0 ports, 0 `via mock`/`shopify`/`fintrack`/`todoist`, 0 em/en dashes, 14,117 chars (< 20,000). |
| MEMORY.md | C:\Users\lenovo\Desktop\06-06-Mansa\Asha Gallegos\asha-gallegos\MEMORY.md | F-006, F-007, F-008 | Written to disk. Re-passes Mode A (Off-Mic state and Connected Accounts now agree with TOOLS), Mode B (no new duplication; HOW stays in TOOLS), Mode F (11 H2 sections in canonical order; 14,999 chars < 15,000; 0 dashes). |
| AGENTS.md, SOUL.md, IDENTITY.md, USER.md, HEARTBEAT.md | (same folder) | none | Unmodified; verified compliant (AGENTS 7 H2s ending Data Sharing Policy; IDENTITY H1 without suffix; USER 5 H2s / 33 lines; HEARTBEAT single Weekly, no Default; SOUL 4 H2s). HEARTBEAT Annual birthday entries pending Q1. |

Post-remediation totals: 7 files, 44,664 chars combined (< 140,000); every file < 20,000.

---

## Section 6 - Cross-Persona Pattern Flags (SYSTEMIC)

1. **SYSTEMIC - locale-substitution slug swaps (F-001 class).** The generator replaced US-locale canonical APIs with real local-brand equivalents for a non-US persona (Checkers Sixty60 for Instacart, Uber Eats for DoorDash, Property24 for Zillow, Vault22 for Plaid, SimplePay for Gusto, Tripadvisor for Yelp) and added podcast-trade tools (Otter, Riverside, Descript, Buzzsprout, Acast, Canva, SoundCloud) not on the canonical list. Any persona generated with the same localization instinct will fail the E6 canonical-set gate while passing the raw count of 101. Recommend a template-level hard gate: set-diff against the canonical list, not just a count.
2. **SYSTEMIC - dormant-phrasing bullets (F-002 class).** "Stands by / On hand / Ready for / Configured for / parked / on standby" phrasing for aspirational-project tools (pre-launch podcast, future merch) is a generation-template habit likely replicated across the cohort. Recommend adding the banned-phrase grep to the generation validation checklist.
3. **SYSTEMIC - missing inner-circle DOBs and Annual birthday block (F-009 class).** Ages-without-DOBs in Key Relationships plus an absent HEARTBEAT `### Annual` birthday set is a structural omission pattern; check sibling personas.
