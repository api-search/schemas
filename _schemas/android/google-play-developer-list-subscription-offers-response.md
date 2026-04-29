---
description: Response containing a list of subscription offers.
layout: schema
name: ListSubscriptionOffersResponse
properties_list:
- description: ''
  name: subscriptionOffers
  type: array
- description: Token for the next page of results.
  name: nextPageToken
  type: string
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-list-subscription-offers-response-schema.json
slug: google-play-developer-list-subscription-offers-response
source_filename: google-play-developer-list-subscription-offers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListSubscriptionOffersResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response containing a list of subscription offers.\",\n  \"properties\": {\n    \"subscriptionOffers\": {\n      \"type\": \"array\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-list-subscription-offers-response-schema.json
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
title: ListSubscriptionOffersResponse
---
