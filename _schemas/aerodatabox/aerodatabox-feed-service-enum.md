---
description: 'Airport feed service defininitions<p>Possible values:</p> <ul> <li><b>0 - FlightSchedules</b>: Flight schedules data feed for this airport (static schedules data without actual updates)</li> <li><b>1 - FlightLiveUpdates</b>: Actual flight status and time updates for this airport</li> <li><b>2 - AdsbUpdates</b>: Flight updates derived from ADS-B data for this airport: runway, actual/estimated time on the runway, call-sign, ModeS 24-bit ICAO code, aircraft registration</li> </ul>'
layout: schema
name: FeedServiceEnum
properties_list: []
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-feed-service-enum-schema.json
slug: aerodatabox-feed-service-enum
source_filename: aerodatabox-feed-service-enum-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-feed-service-enum-schema.json\",\n  \"title\": \"FeedServiceEnum\",\n  \"description\": \"Airport feed service defininitions<p>Possible values:</p>\\r\\n<ul>\\r\\n<li><b>0 - FlightSchedules</b>: Flight schedules data feed for this airport (static schedules data without actual updates)</li>\\r\\n<li><b>1 - FlightLiveUpdates</b>: Actual flight status and time updates for this airport</li>\\r\\n<li><b>2 - AdsbUpdates</b>: Flight updates derived from ADS-B data for this airport: runway, actual/estimated time on the runway, call-sign, ModeS 24-bit ICAO code, aircraft registration</li>\\r\\n</ul>\\r\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FlightSchedules\",\n    \"FlightLiveUpdates\",\n    \"AdsbUpdates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-feed-service-enum-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: FeedServiceEnum
---
