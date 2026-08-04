# ThingSpeak (thingspeak)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

ThingSpeak is an IoT analytics platform from MathWorks that lets devices aggregate, visualize, and analyze live data streams in the cloud. Devices push telemetry to channels via a REST update endpoint or the `mqtt3.thingspeak.com` MQTT broker, and the platform layers in MATLAB Analysis for compute, MATLAB Visualizations for plotting, React for rules, TalkBack for cloud-to-device commands, ThingHTTP for outbound webhooks, and TimeControl for scheduling. ThingSpeak is the only mainstream IoT platform with first-class MATLAB and Simulink integration, making it widely used in academic research, environmental monitoring, smart agriculture, and energy applications. Compatible with Arduino, ESP8266/ESP32, Raspberry Pi, Particle, LoRaWAN gateways, and industrial controllers.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- IoT
- Internet of Things
- Analytics
- Time Series
- MQTT
- MATLAB
- Sensors
- Telemetry

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### ThingSpeak Channels API

List, create, read, update, and delete ThingSpeak channels — the primary container for time-series IoT data. Each channel holds up to eight numeric fields plus latitude, longitude, elevation, and a status string. Channels can be public, private, or shared via read API keys.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/channelsapi.html](https://www.mathworks.com/help/thingspeak/channelsapi.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Channels
- Data
- Analytics

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/channelsapi.html)
- [OpenAPI](openapi/thingspeak-channels-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/thingspeak-channel-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/thingspeak-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### ThingSpeak Feeds API

Read channel feed entries with rich querying — last N results, by date range, by field, with timezone, rounding, averaging, and median/sum aggregation. Supports JSON, XML, and CSV response formats and works with both public channels and private channels via Read API Keys.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/readdata.html](https://www.mathworks.com/help/thingspeak/readdata.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Feeds
- Time Series
- Read

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/readdata.html)
- [OpenAPI](openapi/thingspeak-feeds-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/thingspeak-feed-schema.json) — [JSON Schema](https://json-schema.org/specification)

### ThingSpeak Update API

Write a single channel entry via `/update` or push high-volume telemetry via `/channels/{channel_id}/bulk_update.json` (CSV or JSON batches). The write surface is the workhorse of every ThingSpeak device — Arduino, ESP32, Raspberry Pi, Particle, and any HTTP-capable sensor node.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/writedata.html](https://www.mathworks.com/help/thingspeak/writedata.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Write
- Telemetry

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/writedata.html)
- [Documentation](https://www.mathworks.com/help/thingspeak/bulkwritejsondata.html)
- [OpenAPI](openapi/thingspeak-update-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak MQTT API

Lightweight pub/sub MQTT broker at `mqtt3.thingspeak.com` over TCP (1883), TLS (8883), WebSocket (80), and secure WebSocket (443, path `/mqtt`). Publish to `channels/{channelID}/publish` and subscribe via `channels/{channelID}/subscribe/fields/field{n}/{readAPIKey}`. QoS 0 only; connections time out after one hour of inactivity. Devices use MQTT-specific Client ID / Username / Password credentials provisioned in ThingSpeak.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/mqtt-api.html](https://www.mathworks.com/help/thingspeak/mqtt-api.html)
- **Base URL:** `mqtt3.thingspeak.com`

#### Tags

- IoT
- MQTT
- Pub/Sub
- Real-Time

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/mqtt-api.html)
- [Documentation](https://www.mathworks.com/help/thingspeak/mqtt-basics.html)
- [AsyncAPI](asyncapi/thingspeak-mqtt-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak TalkBack API

Asynchronous command queue letting cloud-side logic or humans push instructions to remote devices. Devices poll `talkbacks/{id}/commands` and execute the next command; commands can be added, updated, executed, or deleted via the REST surface. Pairs naturally with React for closed-loop automation.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/talkbackapp.html](https://www.mathworks.com/help/thingspeak/talkbackapp.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Commands
- Queue
- Device Management

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/talkbackapp.html)
- [OpenAPI](openapi/thingspeak-talkback-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak React API

React lets channels react to incoming data — running ThingHTTP requests, MATLAB Analysis snippets, TalkBack commands, or Twitter/Tweet posts when conditions (numeric threshold, string match, no-data) are met. Configured via the React app UI, this is ThingSpeak's primary rules engine.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/react-app.html](https://www.mathworks.com/help/thingspeak/react-app.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Automation
- Triggers
- Events

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/react-app.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak Alerts API

Send email alerts from a channel via the alerts API or React, and retrieve alert history. Useful for environmental monitoring, threshold-based warnings, and inactivity notifications.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/alerts.html](https://www.mathworks.com/help/thingspeak/alerts.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Alerts
- Email
- Notifications

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/alerts.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak Charts API

Server-rendered chart embeds for any channel/field — line, bar, column, spline — with parameters for color, scale, axis, timezone, title, bgcolor, transparent, and dynamic options. Returns embeddable HTML/SVG.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/charts.html](https://www.mathworks.com/help/thingspeak/charts.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Charts
- Visualization

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/charts.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak MATLAB Analysis API

Run scheduled or React-triggered MATLAB code against channel data — the differentiator that separates ThingSpeak from generic MQTT brokers. Read channel data with `thingSpeakRead`, write results back with `thingSpeakWrite`, and access the standard MATLAB toolboxes (signal processing, statistics, machine learning) inside a managed sandbox.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/matlab-analysis-app.html](https://www.mathworks.com/help/thingspeak/matlab-analysis-app.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- MATLAB
- Analysis
- Compute

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/matlab-analysis-app.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak MATLAB Visualization API

Generate custom plots from MATLAB code and embed them on ThingSpeak channel pages or external dashboards. Supports `plotyy`, `geoplot`, `histogram`, custom colormaps, and any other MATLAB plotting primitive against channel feed data.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/matlab-visualizations-app.html](https://www.mathworks.com/help/thingspeak/matlab-visualizations-app.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- MATLAB
- Visualization

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/matlab-visualizations-app.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak ThingHTTP API

Outbound HTTP requests stored as named "ThingHTTP" actions and fired by React, TimeControl, or device pollers. Lets ThingSpeak push data into third-party services (Twilio, IFTTT, custom webhooks) without a backend server.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/thinghttp-app.html](https://www.mathworks.com/help/thingspeak/thinghttp-app.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Webhooks
- Integrations

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/thinghttp-app.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ThingSpeak TimeControl API

Cron-style scheduler that fires ThingHTTP, TalkBack, or MATLAB Analysis actions at a chosen time, recurring frequency, or after a delay. Pairs with React and TalkBack to close the IoT control loop.

- **Human URL:** [https://www.mathworks.com/help/thingspeak/timecontrolapp.html](https://www.mathworks.com/help/thingspeak/timecontrolapp.html)
- **Base URL:** `https://api.thingspeak.com/`

#### Tags

- IoT
- Scheduling
- Cron

#### Properties

- [Documentation](https://www.mathworks.com/help/thingspeak/timecontrolapp.html)
- [Postman Collection](collections/thingspeak-channels-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-channels-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-feeds-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-feeds-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-talkback-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-talkback-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/thingspeak-update-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thingspeak-update-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://thingspeak.mathworks.com/)
- [Documentation](https://www.mathworks.com/help/thingspeak/)
- [Documentation](https://www.mathworks.com/help/thingspeak/rest-api.html)
- [Documentation](https://www.mathworks.com/help/thingspeak/mqtt-api.html)
- [Getting Started](https://www.mathworks.com/help/thingspeak/get-started-with-thingspeak.html)
- [Sign Up](https://thingspeak.mathworks.com/login)
- [Sign Up](https://www.mathworks.com/mwaccount/register)
- [Pricing](https://thingspeak.mathworks.com/prices)
- [Terms of Service](https://thingspeak.mathworks.com/pages/license_faq)
- [Terms of Service](https://www.mathworks.com/company/aboutus/policies_statements/)
- [Privacy Policy](https://www.mathworks.com/company/aboutus/policies_statements/privacy-policy.html)
- [Support](https://www.mathworks.com/support/contact_us.html)
- [GitHub Organization](https://github.com/mathworks)
- [SDK](https://github.com/mathworks/thingspeak-arduino)
- [SDK](https://github.com/mathworks/thingspeak-particle)
- [SDK](https://www.mathworks.com/matlabcentral/fileexchange/52244-thingspeak-support-from-desktop-matlab)
- [Tutorials](https://www.mathworks.com/help/thingspeak/use-arduino-client-to-publish-to-a-channel.html)
- [Tutorials](https://www.mathworks.com/help/thingspeak/raspberry-pi-tutorials.html)
- [Tutorials](https://www.mathworks.com/help/thingspeak/esp32-tutorials.html)
- [Tutorials](https://www.mathworks.com/help/thingspeak/esp8266-tutorials.html)
- [Tutorials](https://www.mathworks.com/help/thingspeak/particle-photon-tutorials.html)
- [Forum](https://www.mathworks.com/matlabcentral/answers/index?term=tag%3Athingspeak)
- [Community](https://www.mathworks.com/matlabcentral/communitycontests/contests/4/entries)
- [Blog](https://blogs.mathworks.com/iot/)
- [Product Page](https://www.mathworks.com/products/thingspeak.html)
- [LinkedIn](https://www.linkedin.com/company/the-mathworks_2/)
- [X (Twitter)](https://x.com/MATLAB)
- [YouTube](https://www.youtube.com/user/MATLAB)
- [Plans](https://plans/thingspeak-plans-pricing.yml)
- [Rate Limits](https://rate-limits/thingspeak-rate-limits.yml)
- [Fin Ops](https://finops/thingspeak-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
