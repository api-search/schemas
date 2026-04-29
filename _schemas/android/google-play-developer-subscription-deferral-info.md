---
description: Contains the new desired expiry time for a subscription deferral.
layout: schema
name: SubscriptionDeferralInfo
properties_list:
- description: The expected expiry time for the subscription. If the current expiry time does not match, the deferral will not occur.
  name: expectedExpiryTimeMillis
  type: string
- description: The desired next expiry time to assign to the subscription. Must be later than the current expiry time.
  name: desiredExpiryTimeMillis
  type: string
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-subscription-deferral-info-schema.json
slug: google-play-developer-subscription-deferral-info
source_filename: google-play-developer-subscription-deferral-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionDeferralInfo\",\n  \"type\": \"object\",\n  \"description\": \"Contains the new desired expiry time for a subscription deferral.\",\n  \"properties\": {\n    \"expectedExpiryTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"The expected expiry time for the subscription. If the current expiry time does not match, the deferral will not occur.\"\n    },\n    \"desiredExpiryTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"The desired next expiry time to assign to the subscription. Must be later than the current expiry time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-subscription-deferral-info-schema.json
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
title: SubscriptionDeferralInfo
---
