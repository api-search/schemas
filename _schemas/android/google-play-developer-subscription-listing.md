---
description: Localized listing information for a subscription.
layout: schema
name: SubscriptionListing
properties_list:
- description: BCP-47 language tag (e.g., en-US).
  name: languageCode
  type: string
- description: The title of the subscription in this locale.
  name: title
  type: string
- description: A list of benefits shown to the user on platforms such as the Play Store. Limited to four benefits.
  name: benefits
  type: array
- description: The description of the subscription in this locale.
  name: description
  type: string
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-subscription-listing-schema.json
slug: google-play-developer-subscription-listing
source_filename: google-play-developer-subscription-listing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionListing\",\n  \"type\": \"object\",\n  \"description\": \"Localized listing information for a subscription.\",\n  \"properties\": {\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"BCP-47 language tag (e.g., en-US).\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the subscription in this locale.\"\n    },\n    \"benefits\": {\n      \"type\": \"array\",\n      \"description\": \"A list of benefits shown to the user on platforms such as the Play Store. Limited to four benefits.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the subscription in this locale.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-subscription-listing-schema.json
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
title: SubscriptionListing
---
