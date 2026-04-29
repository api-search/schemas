---
description: A timestamp in seconds and nanoseconds.
layout: schema
name: Timestamp
properties_list:
- description: Seconds since Unix Epoch.
  name: seconds
  type: string
- description: Non-negative fractions of a second at nanosecond resolution.
  name: nanos
  type: integer
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-timestamp-schema.json
slug: google-play-developer-timestamp
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Timestamp\",\n  \"type\": \"object\",\n  \"description\": \"A timestamp in seconds and nanoseconds.\",\n  \"properties\": {\n    \"seconds\": {\n      \"type\": \"string\",\n      \"description\": \"Seconds since Unix Epoch.\"\n    },\n    \"nanos\": {\n      \"type\": \"integer\",\n      \"description\": \"Non-negative fractions of a second at nanosecond resolution.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-timestamp-schema.json
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
title: Timestamp
---
