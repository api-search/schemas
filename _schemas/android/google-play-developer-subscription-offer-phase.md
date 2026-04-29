---
description: A single phase of a subscription offer. Defines pricing for a specific period.
layout: schema
name: SubscriptionOfferPhase
properties_list:
- description: The number of times this phase repeats. If 0, the phase repeats indefinitely.
  name: recurrenceCount
  type: integer
- description: Duration of a single period in ISO 8601 format.
  name: duration
  type: string
- description: Regional pricing for this phase.
  name: regionalConfigs
  type: array
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-subscription-offer-phase-schema.json
slug: google-play-developer-subscription-offer-phase
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionOfferPhase\",\n  \"type\": \"object\",\n  \"description\": \"A single phase of a subscription offer. Defines pricing for a specific period.\",\n  \"properties\": {\n    \"recurrenceCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times this phase repeats. If 0, the phase repeats indefinitely.\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"Duration of a single period in ISO 8601 format.\"\n    },\n    \"regionalConfigs\": {\n      \"type\": \"array\",\n      \"description\": \"Regional pricing for this phase.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-subscription-offer-phase-schema.json
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
title: SubscriptionOfferPhase
---
