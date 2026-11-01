# ThingSpeak

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

ThingSpeak is an IoT analytics platform from MathWorks that lets devices aggregate, visualize, and analyze live data streams in the cloud. Devices push telemetry to channels via a REST update endpoint or the `mqtt3.thingspeak.com` MQTT broker, and the platform layers in MATLAB Analysis for compute, MATLAB Visualizations for plotting, React for rules, TalkBack for cloud-to-device commands, ThingHTTP for outbound webhooks, and TimeControl for scheduling. ThingSpeak is the only mainstream IoT platform with first-class MATLAB and Simulink integration, making it widely used in academic research, environmental monitoring, smart agriculture, and energy applications. Compatible with Arduino, ESP8266/ESP32, Raspberry Pi, Particle, LoRaWAN gateways, and industrial controllers.

**Areas:** IoT · Analytics · Time Series · MQTT · MATLAB · Sensors · Telemetry · Real-Time

## ThingSpeak on APIs.io

Everything profiled for ThingSpeak is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/thingspeak/](https://apis.io/providers/thingspeak/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [ThingSpeak Channels API](https://apis.io/apis/thingspeak/thingspeak-channels-api/) — List, create, read, update, and delete ThingSpeak channels — the primary container for time-series IoT data. Each channel holds up to eight numeric fields…
- [ThingSpeak Update API](https://apis.io/apis/thingspeak/thingspeak-update-api/) — Write a single channel entry via `/update` or push high-volume telemetry via `/channels/{channel_id}/bulk_update.json` (CSV or JSON batches). The write…
- [ThingSpeak MQTT API](https://apis.io/apis/thingspeak/thingspeak-mqtt-api/) — Lightweight pub/sub MQTT broker at `mqtt3.thingspeak.com` over TCP (1883), TLS (8883), WebSocket (80), and secure WebSocket (443, path `/mqtt`). Publish to…
- [ThingSpeak React API](https://apis.io/apis/thingspeak/thingspeak-react-api/) — React lets channels react to incoming data — running ThingHTTP requests, MATLAB Analysis snippets, TalkBack commands, or Twitter/Tweet posts when conditions…
- [ThingSpeak Alerts API](https://apis.io/apis/thingspeak/thingspeak-alerts-api/) — Send email alerts from a channel via the alerts API or React, and retrieve alert history. Useful for environmental monitoring, threshold-based warnings, and…
- [ThingSpeak Charts API](https://apis.io/apis/thingspeak/thingspeak-charts-api/) — Server-rendered chart embeds for any channel/field — line, bar, column, spline — with parameters for color, scale, axis, timezone, title, bgcolor,…
- [ThingSpeak MATLAB Analysis API](https://apis.io/apis/thingspeak/thingspeak-matlab-analysis-api/) — Run scheduled or React-triggered MATLAB code against channel data — the differentiator that separates ThingSpeak from generic MQTT brokers. Read channel…
- [ThingSpeak MATLAB Visualization API](https://apis.io/apis/thingspeak/thingspeak-matlab-visualization-api/) — Generate custom plots from MATLAB code and embed them on ThingSpeak channel pages or external dashboards. Supports `plotyy`, `geoplot`, `histogram`, custom…
- [ThingSpeak ThingHTTP API](https://apis.io/apis/thingspeak/thingspeak-thinghttp-api/) — Outbound HTTP requests stored as named "ThingHTTP" actions and fired by React, TimeControl, or device pollers. Lets ThingSpeak push data into third-party…
- [ThingSpeak TimeControl API](https://apis.io/apis/thingspeak/thingspeak-timecontrol-api/) — Cron-style scheduler that fires ThingHTTP, TalkBack, or MATLAB Analysis actions at a chosen time, recurring frequency, or after a delay. Pairs with React…
- [ThingSpeak Channels.json API](https://apis.io/apis/thingspeak/thingspeak-channels-json-api/) — The Channels.json API from ThingSpeak — 1 operation(s) for channels.json.
- [ThingSpeak Talkbacks API](https://apis.io/apis/thingspeak/thingspeak-talkbacks-api/) — The Talkbacks API from ThingSpeak — 3 operation(s) for talkbacks.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (12)

Multi-step workflows that chain operations into a business task.

- [ThingSpeak Bulk Update and Read Field Feed](https://apis.io/arazzos/thingspeak/thingspeak-bulk-update-and-read-field-feed-workflow/)
- [ThingSpeak Decommission Channel](https://apis.io/arazzos/thingspeak/thingspeak-decommission-channel-workflow/)
- [ThingSpeak Discover Public Channel and Read Feed](https://apis.io/arazzos/thingspeak/thingspeak-discover-public-channel-and-read-feed-workflow/)
- [ThingSpeak Inspect Channel and Aggregate Feed](https://apis.io/arazzos/thingspeak/thingspeak-inspect-channel-and-aggregate-feed-workflow/)
- [ThingSpeak List Channels and Read Feed](https://apis.io/arazzos/thingspeak/thingspeak-list-channels-and-read-feed-workflow/)
- [ThingSpeak Post Status and Read Status Updates](https://apis.io/arazzos/thingspeak/thingspeak-post-status-and-read-status-updates-workflow/)
- [ThingSpeak Provision Channel and Seed First Reading](https://apis.io/arazzos/thingspeak/thingspeak-provision-channel-and-seed-reading-workflow/)
- [ThingSpeak Queue and Execute TalkBack Command](https://apis.io/arazzos/thingspeak/thingspeak-queue-and-execute-talkback-command-workflow/)
- [ThingSpeak Relabel Field and Read Last Field Entry](https://apis.io/arazzos/thingspeak/thingspeak-relabel-field-and-read-last-field-entry-workflow/)
- [ThingSpeak Revise Queued TalkBack Command](https://apis.io/arazzos/thingspeak/thingspeak-revise-queued-talkback-command-workflow/)
- [ThingSpeak Sweep Executed TalkBack Commands](https://apis.io/arazzos/thingspeak/thingspeak-sweep-executed-talkback-commands-workflow/)
- [ThingSpeak Write Update and Read Last Entry](https://apis.io/arazzos/thingspeak/thingspeak-write-update-and-read-last-entry-workflow/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [ThingSpeak MQTT API](https://apis.io/asyncapis/thingspeak/thingspeak-mqtt-asyncapi/)

#### Event channels (4)

Individual events and webhooks the provider emits.

- [channels/{channelID}/publish](https://apis.io/channels/thingspeak/channels-channelid-publish/)
- [channels/{channelID}/publish/fields/field{fieldNumber}](https://apis.io/channels/thingspeak/channels-channelid-publish-fields-field-fieldnumber/)
- [channels/{channelID}/subscribe/fields/field{fieldNumber}/{readAPIKey}](https://apis.io/channels/thingspeak/channels-channelid-subscribe-fields-field-fieldnumber-readapikey/)
- [channels/{channelID}/subscribe/json/{readAPIKey}](https://apis.io/channels/thingspeak/channels-channelid-subscribe-json-readapikey/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Thingspeak Agentic Access](https://apis.io/agentic-access/thingspeak/thingspeak-agentic-access/)

#### JSON Schema (2)

The data models the API reads and writes.

- [ThingSpeak Channel](https://apis.io/schemas/thingspeak/thingspeak-channel/)
- [ThingSpeak Feed Entry](https://apis.io/schemas/thingspeak/thingspeak-feed/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Thingspeak Context](https://apis.io/jsonld/thingspeak/thingspeak-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Thingspeak Vocabulary](https://apis.io/vocabularies/thingspeak/thingspeak-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Thingspeak Bulk Update Example](https://apis.io/examples/thingspeak/thingspeak-bulk-update-example/)
- [Thingspeak Mqtt Publish Example](https://apis.io/examples/thingspeak/thingspeak-mqtt-publish-example/)
- [Thingspeak Read Channel Feed Example](https://apis.io/examples/thingspeak/thingspeak-read-channel-feed-example/)
- [Thingspeak Talkback Execute Example](https://apis.io/examples/thingspeak/thingspeak-talkback-execute-example/)
- [Thingspeak Update Channel Example](https://apis.io/examples/thingspeak/thingspeak-update-channel-example/)

#### Collections (10)

Postman and Open Collection request collections.

- [ThingSpeak Channels API](https://apis.io/collections/thingspeak/open-thingspeak-channels-api/)
- [ThingSpeak Channels Channels.json API](https://apis.io/collections/thingspeak/open-thingspeak-channels-json-api/)
- [ThingSpeak Feeds API](https://apis.io/collections/thingspeak/open-thingspeak-feeds-api/)
- [ThingSpeak TalkBack API](https://apis.io/collections/thingspeak/open-thingspeak-talkback-api/)
- [ThingSpeak Channels Talkbacks API](https://apis.io/collections/thingspeak/open-thingspeak-talkbacks-api/)
- [ThingSpeak Channels Update API](https://apis.io/collections/thingspeak/open-thingspeak-update-api/)
- [ThingSpeak Channels API](https://apis.io/collections/thingspeak/postman-thingspeak-channels-api/)
- [ThingSpeak Feeds API](https://apis.io/collections/thingspeak/postman-thingspeak-feeds-api/)
- [ThingSpeak TalkBack API](https://apis.io/collections/thingspeak/postman-thingspeak-talkback-api/)
- [ThingSpeak Update API](https://apis.io/collections/thingspeak/postman-thingspeak-update-api/)

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [ThingSpeak — asyncapi rules](https://apis.io/rules/thingspeak/thingspeak-asyncapi-spectral-rules/)
- [ThingSpeak — jsonschema rules](https://apis.io/rules/thingspeak/thingspeak-jsonschema-spectral-rules/)
- [ThingSpeak API Rules](https://apis.io/rules/thingspeak/thingspeak-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Thingspeak Authentication](https://apis.io/security/thingspeak/thingspeak-authentication/)
- [Thingspeak Domain Security](https://apis.io/security/thingspeak/thingspeak-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Thingspeak Plans Pricing](https://apis.io/plans/thingspeak/thingspeak-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Thingspeak Rate Limits](https://apis.io/rate-limits/thingspeak/thingspeak-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Thingspeak Finops](https://apis.io/finops/thingspeak/thingspeak-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Documentation](https://www.mathworks.com/help/thingspeak/)
- [Getting started](https://www.mathworks.com/help/thingspeak/get-started-with-thingspeak.html)
- [Pricing](https://thingspeak.mathworks.com/prices)
- [Support](https://www.mathworks.com/support/contact_us.html)
- [Blog](https://blogs.mathworks.com/iot/)
- [Terms of service](https://thingspeak.mathworks.com/pages/license_faq)
- [Privacy policy](https://www.mathworks.com/company/aboutus/policies_statements/privacy-policy.html)
- [GitHub](https://github.com/mathworks)

## API Evangelist rating

**Unrated** — no public website could be reached for this company, so there was almost nothing to measure and nothing a reader could check.

This is not a score of zero. No rating is published for this company. If that is wrong because something public exists that we missed, say so on this repository or email [info@apievangelist.com](mailto:info@apievangelist.com) and it will be re-run — free, and no justification needed.

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for ThingSpeak: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/thingspeak/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
