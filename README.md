# ThingSpeak (thingspeak)
ThingSpeak is an IoT analytics platform from MathWorks that lets devices aggregate, visualize, and analyze live data streams in the cloud. Devices push telemetry to channels via a REST update endpoint or the `mqtt3.thingspeak.com` MQTT broker, and the platform layers in MATLAB Analysis for compute, MATLAB Visualizations for plotting, React for rules, TalkBack for cloud-to-device commands, ThingHTTP for outbound webhooks, and TimeControl for scheduling. ThingSpeak is the only mainstream IoT platform with first-class MATLAB and Simulink integration.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/thingspeak/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - IoT, Internet of Things, Analytics, Time Series, MQTT, MATLAB, Sensors, Telemetry

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### ThingSpeak Channels API
Create, list, update, and delete channels — the primary container for time-series IoT data. Each channel holds up to eight numeric fields plus latitude, longitude, elevation, and a status string.

**Human URL:** [https://www.mathworks.com/help/thingspeak/channelsapi.html](https://www.mathworks.com/help/thingspeak/channelsapi.html)

- [Documentation](https://www.mathworks.com/help/thingspeak/channelsapi.html)
- [OpenAPI](openapi/thingspeak-channels-api-openapi.yml)
- [JSON Schema — Channel](json-schema/thingspeak-channel-schema.json)
- [JSON-LD](json-ld/thingspeak-context.jsonld)
- [Naftiko Capability — Channels](capabilities/channels-channels.yaml)

### ThingSpeak Feeds API
Read channel feed entries with rich query support — last N, by date range, by field, with averaging/median/sum aggregation and timezone control. Supports JSON, XML, and CSV.

**Human URL:** [https://www.mathworks.com/help/thingspeak/readdata.html](https://www.mathworks.com/help/thingspeak/readdata.html)

- [OpenAPI](openapi/thingspeak-feeds-api-openapi.yml)
- [JSON Schema — Feed Entry](json-schema/thingspeak-feed-schema.json)
- [Naftiko Capability — Feeds](capabilities/feeds-feeds.yaml)

### ThingSpeak Update API
Write a single channel entry via `/update` or push high-volume telemetry via `/channels/{channel_id}/bulk_update.json` (CSV or JSON batches). The write surface is the workhorse of every ThingSpeak device — Arduino, ESP32, Raspberry Pi, Particle, and any HTTP-capable sensor node.

**Human URL:** [https://www.mathworks.com/help/thingspeak/writedata.html](https://www.mathworks.com/help/thingspeak/writedata.html)

- [OpenAPI](openapi/thingspeak-update-api-openapi.yml)
- [Naftiko Capability — Update](capabilities/update-update.yaml)

### ThingSpeak MQTT API
Lightweight pub/sub broker at `mqtt3.thingspeak.com` over TCP (1883), TLS (8883), WebSocket (80), and secure WebSocket (443, path `/mqtt`). Publish to `channels/{channelID}/publish` and subscribe via `channels/{channelID}/subscribe/fields/field{n}/{readAPIKey}`. QoS 0 only; one-hour inactivity timeout.

**Human URL:** [https://www.mathworks.com/help/thingspeak/mqtt-api.html](https://www.mathworks.com/help/thingspeak/mqtt-api.html)

- [AsyncAPI](asyncapi/thingspeak-mqtt-asyncapi.yml)

### ThingSpeak TalkBack API
Asynchronous command queue letting cloud-side logic push instructions to remote devices. Devices poll `talkbacks/{id}/commands` and execute the next command.

**Human URL:** [https://www.mathworks.com/help/thingspeak/talkbackapp.html](https://www.mathworks.com/help/thingspeak/talkbackapp.html)

- [OpenAPI](openapi/thingspeak-talkback-api-openapi.yml)
- [Naftiko Capability — Commands](capabilities/talkback-commands.yaml)

### ThingSpeak React API
React watches channel data and fires ThingHTTP, MATLAB Analysis, TalkBack, or social posts when threshold, string-match, or no-data conditions are met. The platform's primary rules engine.

**Human URL:** [https://www.mathworks.com/help/thingspeak/react-app.html](https://www.mathworks.com/help/thingspeak/react-app.html)

### ThingSpeak Alerts API
Send email alerts from channels via the alerts API or React, and retrieve alert history.

**Human URL:** [https://www.mathworks.com/help/thingspeak/alerts.html](https://www.mathworks.com/help/thingspeak/alerts.html)

### ThingSpeak Charts API
Server-rendered chart embeds for any channel/field — line, bar, column, spline — with color, scale, axis, timezone, and dynamic options.

**Human URL:** [https://www.mathworks.com/help/thingspeak/charts.html](https://www.mathworks.com/help/thingspeak/charts.html)

### ThingSpeak MATLAB Analysis API
The differentiator that separates ThingSpeak from generic MQTT brokers. Run scheduled or React-triggered MATLAB code against channel data, read with `thingSpeakRead`, write back with `thingSpeakWrite`, and access signal-processing, statistics, and machine-learning toolboxes inside a managed sandbox.

**Human URL:** [https://www.mathworks.com/help/thingspeak/matlab-analysis-app.html](https://www.mathworks.com/help/thingspeak/matlab-analysis-app.html)

### ThingSpeak MATLAB Visualization API
Generate custom plots from MATLAB code and embed them on ThingSpeak channel pages or external dashboards.

**Human URL:** [https://www.mathworks.com/help/thingspeak/matlab-visualizations-app.html](https://www.mathworks.com/help/thingspeak/matlab-visualizations-app.html)

### ThingSpeak ThingHTTP API
Outbound HTTP requests stored as named ThingHTTP actions and fired by React, TimeControl, or device pollers. Push data into Twilio, IFTTT, or any webhook target without a backend.

**Human URL:** [https://www.mathworks.com/help/thingspeak/thinghttp-app.html](https://www.mathworks.com/help/thingspeak/thinghttp-app.html)

### ThingSpeak TimeControl API
Cron-style scheduler that fires ThingHTTP, TalkBack, or MATLAB Analysis at a chosen time, recurring frequency, or after a delay. Closes the IoT control loop with React and TalkBack.

**Human URL:** [https://www.mathworks.com/help/thingspeak/timecontrolapp.html](https://www.mathworks.com/help/thingspeak/timecontrolapp.html)

## Plans

| Plan | Annual Messages | Audience |
|---|---|---|
| Free | ~3M (~8,200/day) | Non-commercial small projects |
| Standard | 33M per unit (~90,400/day) | Commercial, government, organizational |
| Home | 33M per unit | Personal use only |
| Academic | 33M per unit | Teaching/research at degree-granting institutions |
| Student | 33M per unit | Coursework at degree-granting institutions |

See [plans/thingspeak-plans-pricing.yml](plans/thingspeak-plans-pricing.yml), [rate-limits/thingspeak-rate-limits.yml](rate-limits/thingspeak-rate-limits.yml), and [finops/thingspeak-finops.yml](finops/thingspeak-finops.yml).

## SDKs and Tools

- [thingspeak-arduino](https://github.com/mathworks/thingspeak-arduino) — Communication library for Arduino, ESP8266, and ESP32 (C++)
- [thingspeak-particle](https://github.com/mathworks/thingspeak-particle) — Communication library for Particle devices (C++)
- [ThingSpeak Support from Desktop MATLAB](https://www.mathworks.com/matlabcentral/fileexchange/52244-thingspeak-support-from-desktop-matlab) — Read/write from MATLAB on the desktop

## Maintainers

- **Kin Lane** — [API Evangelist](https://apievangelist.com) — info@apievangelist.com
