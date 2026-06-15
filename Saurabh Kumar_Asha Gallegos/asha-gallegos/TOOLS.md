# Tools: Asha Gallegos

## Tool Usage

### Connected Services

#### Show Production & Planning

- **Notion** (`notion-api`): Show rundown templates, the segment archive, and the running ideas board for The Asha Show.
- **Obsidian** (`obsidian-api`): Story lead vault and interview question drafts, linked by theme so old threads resurface when relevant.
- **Airtable** (`airtable-api`): Guest database with topics, availability, and past appearances; the first stop before any booking suggestion.
- **Trello** (`trello-api`): Voices of the City pipeline, from listener nomination to aired profile.
- **Asana** (`asana-api`): Task tracking for the Rhythm FM 30th anniversary documentary series she is building with Sipho.
- **Monday** (`monday-api`): Station campaign boards Dr. Khumalo's team shares for cross-promotion weeks; Asha updates her show's deliverables on them every Friday.
- **Linear** (`linear-api`): Tracks Off-Mic production work: pilot edits, guest shortlists, and launch checklist items, each pinned to a target week.
- **Jira** (`jira-api`): Kgosi Media's ticket queue for studio equipment faults; Naledi files most of them, Asha follows hers.
- **Confluence** (`confluence-api`): Station programming wiki; she checks format clocks and compliance notes there before planning any special segment.
- **Calendly** (`calendly-api`): Guest booking slots for pre-interviews, kept clear of her on-air and prep windows.
- **Typeform** (`typeform-api`): Listener story submission form feeding Voices of the City nominations.

#### Communication & Messaging

- **Gmail** (`gmail-api`): Primary inbox for professional traffic: guests, station management, industry contacts, and event invitations.
- **Outlook** (`outlook-api`): Kgosi Media's corporate account for HR notices and group-wide memos; checked, never lived in.
- **WhatsApp** (`whatsapp-api`): Her main personal channel: the family group, Kagiso, Palesa, and quick coordination with Sipho.
- **Telegram** (`telegram-api`): A few industry group chats where South African radio people trade news and job leads.
- **Slack** (`slack-api`): Rhythm FM production workspace for rundown changes and morning show logistics.
- **Microsoft Teams** (`microsoft-teams-api`): Kgosi Media group meetings and quarterly town halls.
- **Zoom** (`zoom-api`): Remote guest pre-interviews and JMU mentorship check-ins when students cannot travel.
- **Twilio** (`twilio-api`): SMS reminders to confirmed guests the evening before their slot, sent only after Asha approves the booking.

#### Social & Audience

- **Instagram** (`instagram-api`): Her main public-facing platform; drafts and mention monitoring only, nothing publishes without her.
- **Twitter** (`twitter-api`): Live show conversation and breaking news monitoring; any posts are drafted and held for her review.
- **YouTube** (`youtube-api`): Rhythm FM's channel for show clips; tracks comments on her segments.
- **Twitch** (`twitch-api`): She studies how younger broadcasters run live audience chat, pulling format ideas for Off-Mic's interactive segments.
- **Reddit** (`reddit-api`): Johannesburg and South African media subreddits, mined for story leads and listener sentiment.
- **Pinterest** (`pinterest-api`): Mood boards for Off-Mic visual branding and the cottage garden upgrade.
- **LinkedIn** (`linkedin-api`): Industry profile upkeep and incoming speaker requests, summarized weekly.
- **Discord** (`discord-api`): A small South African podcasters server where she trades production tips and tests episode title ideas.

#### Listener Outreach & CRM

- **Mailchimp** (`mailchimp-api`): The Off-Mic newsletter list; collects signups from the landing page and carries her monthly teaser note.
- **Klaviyo** (`klaviyo-api`): Email flows for the Off-Mic supporter shop: order confirmations and restock notes for her vinyl listings.
- **ActiveCampaign** (`activecampaign-api`): Runs the automated welcome series that greets every new Off-Mic newsletter signup with the show's origin story.
- **SendGrid** (`sendgrid-api`): Transactional sends for event RSVPs, like the listener appreciation evening.
- **Mailgun** (`mailgun-api`): Delivery rails for bulk listener mail, including Voices of the City nomination confirmations.
- **HubSpot** (`hubspot-api`): Light CRM for speaking engagements and sponsorship inquiries that come to her directly.
- **Intercom** (`intercom-api`): Powers the listener Q&A widget on the Off-Mic landing page; questions feed straight into episode planning.
- **Zendesk** (`zendesk-api`): Station listener-complaint queue; she reads tickets about her show to spot recurring gripes.
- **Freshdesk** (`freshdesk-api`): Off-Mic's own support inbox; listener questions and guest pitches arrive as tickets, kept separate from the station's Zendesk.
- **Salesforce** (`salesforce-api`): Rhythm FM's sponsor CRM; she reviews which advertisers touch her show before planning sponsored segments.

#### Off-Mic Podcast, Web & Analytics

- **WordPress** (`wordpress-api`): Hosts the Off-Mic show-notes archive and her book-research blog; new posts go up as pilots and chapters progress.
- **Webflow** (`webflow-api`): Runs the live Off-Mic landing page with the newsletter signup form; she tweaks the copy herself after each feedback round.
- **Contentful** (`contentful-api`): Structured episode metadata and guest bios feeding the landing page, so every pilot carries consistent credits.
- **Figma** (`figma-api`): Off-Mic cover art and brand drafts; she comments with strong opinions while a designer friend pushes the pixels.
- **Vimeo** (`vimeo-api`): Hosts Kagiso's screener links and the Off-Mic video trailer she shares with prospective guests.
- **Cloudflare** (`cloudflare-api`): Domain and DNS for the Off-Mic site, set up early so launch day is boring.
- **Algolia** (`algolia-api`): Indexes the show-notes archive and pilot transcripts so site search works from day one.
- **Google Analytics** (`google-analytics-api`): Site traffic for the podcast landing page and newsletter signup conversions.
- **Mixpanel** (`mixpanel-api`): Tracks the signup funnel on the landing page: visit, scroll, form start, confirmed subscriber.
- **Amplitude** (`amplitude-api`): Retention curves for the two private Off-Mic pilots shared with trusted listeners; she checks which segments hold attention.
- **PostHog** (`posthog-api`): Session replays and heatmaps on the landing page; it caught the signup form bug that was costing mobile subscribers.
- **Segment** (`segment-api`): Routes landing-page events to Google Analytics, Mixpanel, and Amplitude so each tool gets wired exactly once.
- **Sentry** (`sentry-api`): Error alerts for the landing page and signup form; she hears about breakage before listeners notice.
- **Datadog** (`datadog-api`): Uptime monitors for the Off-Mic site and the Rhythm FM web stream she checks before going on air.
- **PagerDuty** (`pagerduty-api`): Pages her phone if the Off-Mic site goes down overnight, wired to the Datadog and Cloudflare alerts.

#### Station Systems, HR & Mentorship

- **GitHub** (`github-api`): Naledi's open-source radio automation scripts live here; Asha files feature requests and reads release notes before studio upgrades.
- **GitLab** (`gitlab-api`): Her JMU mentorship students host their data-journalism projects here; she reviews their work and leaves feedback before showcases.
- **Kubernetes** (`kubernetes-api`): Kgosi Media's web stream runs on a Kubernetes cluster; she checks stream service status when listeners report dropouts, before escalating to IT.
- **Okta** (`okta-api`): Single sign-on for station systems; password resets and access requests route through it.
- **ServiceNow** (`servicenow-api`): Kgosi Media facilities requests, like the studio aircon that dies every summer.
- **BambooHR** (`bamboohr-api`): Leave balance and HR documents at Kgosi Media; her leave days never keep pace with her travel list.
- **Greenhouse** (`greenhouse-api`): Station hiring pipelines; she sits on interview panels for on-air roles.
- **Google Classroom** (`google-classroom-api`): JMU Youth Media Mentorship materials and assignments for the current cohort.

#### Money & Finance

- **QuickBooks** (`quickbooks-api`): Tracks appearance fees and speaking income separately from salary, with receipts attached for tax season.
- **Xero** (`xero-api`): The Off-Mic business books: setup costs, pilot expenses, and early supporter income, kept apart from personal finances.
- **Plaid** (`plaid-api`): Feeds her Stripe and PayPal payout accounts into the Off-Mic books so foreign income reconciles without manual entry.
- **Stripe** (`stripe-api`): Processes early-supporter pledges for Off-Mic and the paid newsletter tier.
- **PayPal** (`paypal-api`): Receives occasional international speaking fees and pays the odd overseas vinyl seller.
- **Square** (`square-api`): Card payments at live events; it ran the merch table at the last station fundraiser and handles the listener appreciation evening.
- **Gusto** (`gusto-api`): Runs contractor payments for the US-based audio editor who cuts the Off-Mic pilots.
- **Coinbase** (`coinbase-api`): A tiny experimental holding she checks quarterly and refuses to enlarge.
- **Binance** (`binance-api`): Holds the rand-denominated half of her small crypto experiment; she reviews it alongside Coinbase each quarter.
- **Kraken** (`kraken-api`): Price reference for the show's quarterly money segment; she pulls exchange comparisons before crypto questions go to air.
- **Alpaca** (`alpaca-api`): Paper-trading account she uses to follow a JSE-versus-US-markets segment idea; no real money in it.

#### Calendar, Files & Documents

- **Google Calendar** (`google-calendar-api`): The master schedule: show blocks, guest slots, coaching, therapy, and family commitments.
- **Google Drive** (`google-drive-api`): Show prep documents, interview questions, podcast pitch drafts, and personal records.
- **Dropbox** (`dropbox-api`): Where Kagiso shares rough cuts and where large audio files land from Mandla.
- **Box** (`box-api`): Kgosi Media's official document store for contracts and compliance paperwork.
- **DocuSign** (`docusign-api`): Appearance contracts and release forms for Voices of the City guests.

#### Music, Wellness & Everyday Life

- **Spotify** (`spotify-api`): Daily listening and playlist research: Latin jazz, salsa, cumbia, neo-soul, and new South African artists worth airtime.
- **TMDB** (`tmdb-api`): Documentary lookups for the films Kagiso mentions and the ones she argues with on the couch.
- **OpenLibrary** (`openlibrary-api`): Tracks her South African nonfiction reading list and sources for the radio culture book proposal.
- **NASA** (`nasa-api`): Astronomy picture of the day, an occasional show closer when Johannesburg needs a little wonder.
- **MyFitnessPal** (`myfitnesspal-api`): Loose habit tracking around training weeks; consistency patterns, never calorie pressure.
- **Strava** (`strava-api`): Logs Melville Running Club sessions and training runs.

#### City Life, Travel & Events

- **Google Maps** (`google-maps-api`): Johannesburg routing, guest pickup logistics, and travel time math against the 5:00 AM station arrival.
- **OpenWeather** (`openweather-api`): Morning weather for the show's traffic-and-weather beats and for run planning.
- **Uber** (`uber-api`): Rides for guests coming to the studio and for nights out when the Polo stays home.
- **Yelp** (`yelp-api`): Restaurant and venue shortlists for the US podcast-conference trip she is building around Off-Mic launch networking.
- **Zillow** (`zillow-api`): US housing data for the show's monthly property-affordability segment, set against the Joburg deposit math she lives herself.
- **Instacart** (`instacart-api`): US grocery-basket price pulls for the show's cost-of-living comparisons between Joburg staples and American cities.
- **DoorDash** (`doordash-api`): US delivery-economy data feeding a Voices of the City series on Joburg's couriers and gig work.
- **Ticketmaster** (`ticketmaster-api`): Concert tickets, both for joy and for gifting; experiences are her default present.
- **Eventbrite** (`eventbrite-api`): Community event listings for show coverage and registration for industry functions.
- **Airbnb** (`airbnb-api`): Stays for Cape Town drives and the someday Colombia trip she keeps in the future tense.
- **Amadeus** (`amadeus-api`): Flight options for work trips; window seats only, so the shade stays under her control.
- **Ring** (`ring-api`): Cottage doorbell camera; alerts checked after early departures leave the house empty before dawn.

#### Shopping & Shipping

- **Amazon Seller** (`amazon-seller-api`): Sells duplicate pressings from her vinyl collection to international collectors; listings rotate as the crates get re-sorted.
- **Etsy** (`etsy-api`): Sources statement jewelry and African-print fabric finds, plus gifts for Sofia and Palesa.
- **BigCommerce** (`bigcommerce-api`): Powers the Voices of the City community merch pilot, with proceeds routed to featured community organizations.
- **WooCommerce** (`woocommerce-api`): Runs the Off-Mic supporter shop bolted onto the WordPress site: presale notebooks, stickers, and early-supporter bundles.
- **Shippo** (`shippo-api`): Prints shipping labels for vinyl sales and supporter-shop orders headed overseas.
- **FedEx** (`fedex-api`): Tracks international vinyl shipments from overseas sellers.
- **UPS** (`ups-api`): Tracks studio equipment orders, including the podcast microphones currently working through customs.

#### Not Connected

- Live web search, web browsing, and deep internet research are not available. The assistant works only from connected services and stored memory.
- Rhythm FM and Kgosi Media internal broadcast systems (playout and ad traffic) are not connected; show commitments are tracked from what Asha shares.
- Kagiso's accounts, Carmen's accounts, and the family WhatsApp group admin controls stay outside the assistant's reach.
- No station payroll or salary systems; her salary and her own contract terms exist only as facts Asha has shared.
