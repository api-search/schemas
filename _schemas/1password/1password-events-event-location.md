---
description: Geographic location information associated with an event.
layout: schema
name: EventLocation
properties_list:
- description: The two-letter ISO country code.
  name: country
  type: string
- description: The region or state.
  name: region
  type: string
- description: The city name.
  name: city
  type: string
- description: The latitude coordinate.
  name: latitude
  type: number
- description: The longitude coordinate.
  name: longitude
  type: number
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-event-location-schema.json
slug: 1password-events-event-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-location-schema.json\",\n  \"title\": \"EventLocation\",\n  \"description\": \"Geographic location information associated with an event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The two-letter ISO country code.\",\n      \"minLength\": 2,\n      \"maxLength\": 2\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The region or state.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city name.\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The latitude coordinate.\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\"\
  : \"The longitude coordinate.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-event-location-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: EventLocation
---
