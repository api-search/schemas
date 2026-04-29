---
description: Airport data feed services status. Read https://aerodatabox.com/data-coverage for context.
layout: schema
name: AirportFeedServiceStatusContract
properties_list:
- description: ''
  name: flightSchedulesFeed
  type: object
- description: ''
  name: liveFlightUpdatesFeed
  type: object
- description: ''
  name: adsbUpdatesFeed
  type: object
- description: ''
  name: generalAvailability
  type: object
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-airport-feed-service-status-contract-schema.json
slug: aerodatabox-airport-feed-service-status-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-feed-service-status-contract-schema.json\",\n  \"title\": \"AirportFeedServiceStatusContract\",\n  \"description\": \"Airport data feed services status.\\r\\nRead https://aerodatabox.com/data-coverage for context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flightSchedulesFeed\": {\n      \"$ref\": \"#/components/schemas/FeedServiceStatusContract\"\n    },\n    \"liveFlightUpdatesFeed\": {\n      \"$ref\": \"#/components/schemas/FeedServiceStatusContract\"\n    },\n    \"adsbUpdatesFeed\": {\n      \"$ref\": \"#/components/schemas/FeedServiceStatusContract\"\n    },\n    \"generalAvailability\": {\n      \"$ref\": \"#/components/schemas/FlightDataGeneralAvailabilityContract\"\n    }\n  },\n  \"required\": [\n    \"adsbUpdatesFeed\",\n    \"flightSchedulesFeed\",\n    \"generalAvailability\"\
  ,\n    \"liveFlightUpdatesFeed\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-airport-feed-service-status-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: AirportFeedServiceStatusContract
---
