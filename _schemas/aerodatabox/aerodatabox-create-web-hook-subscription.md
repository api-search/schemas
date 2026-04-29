---
description: Command to create web-hook subscription
layout: schema
name: CreateWebHookSubscription
properties_list:
- description: 'Destination HTTP-endpoint where notifications will be sent to. Requirements: * must be a valid public HTTP(S) URL not requiring additional authorization; * must use standard or alternative HTTP or HTT'
  name: url
  type: string
- description: 'Maximum number of times a delivery attempt is retried after initial delivery attempt failure. Current default value is: * `2` for the old, lifetime-based web-hook subscriptions (will be phased out aft'
  name: maxDeliveryRetries
  type: integer
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-create-web-hook-subscription-schema.json
slug: aerodatabox-create-web-hook-subscription
source_filename: aerodatabox-create-web-hook-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-create-web-hook-subscription-schema.json\",\n  \"title\": \"CreateWebHookSubscription\",\n  \"description\": \"Command to create web-hook subscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"Destination HTTP-endpoint where notifications will be sent to. Requirements:\\r\\n* must be a valid public HTTP(S) URL not requiring additional authorization;\\r\\n* must use standard or alternative HTTP or HTTPS ports (80, 443, 8008, 8080) or any dynamic port greater or equal to 49152;\\r\\n* must be able to accept HTTP POST request with JSON-formatted body (application/json);\\r\\n* must respond with one of successful HTTP status codes (2XX) within 10 seconds;\\r\\n* the endpoint owner must be aware of\
  \ and consent to receiving notifications at it.\\r\\n\\r\\nIf endpoint is unavailable, responds with error status code or does not respond within timeout,\\r\\nnotification delivery retry may be attempted according to subscription settings.\"\n    },\n    \"maxDeliveryRetries\": {\n      \"maximum\": 2,\n      \"minimum\": 0,\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of times a delivery attempt is retried after initial delivery attempt failure.\\r\\n\\r\\nCurrent default value is:\\r\\n\\r\\n\\t* `2` for the old, lifetime-based web-hook subscriptions (will be phased out after the 4th of April, 2026);\\r\\n\\t* `0` for the new, credit-based web-hook subscriptions (will be the default value for any web-hook subscription after the 4th of April, 2026).\",\n      \"format\": \"int32\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"url\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-create-web-hook-subscription-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: CreateWebHookSubscription
---
