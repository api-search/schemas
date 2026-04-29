---
description: Contains the introductory price information for a subscription.
layout: schema
name: IntroductoryPriceInfo
properties_list:
- description: ISO 4217 currency code for the introductory price.
  name: introductoryPriceCurrencyCode
  type: string
- description: Introductory price in micro-units of the currency.
  name: introductoryPriceAmountMicros
  type: string
- description: Introductory price period in ISO 8601 format (e.g., P1W for one week, P1M for one month).
  name: introductoryPricePeriod
  type: string
- description: Number of billing periods the introductory price applies for.
  name: introductoryPriceCycles
  type: integer
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-introductory-price-info-schema.json
slug: google-play-developer-introductory-price-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntroductoryPriceInfo\",\n  \"type\": \"object\",\n  \"description\": \"Contains the introductory price information for a subscription.\",\n  \"properties\": {\n    \"introductoryPriceCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the introductory price.\"\n    },\n    \"introductoryPriceAmountMicros\": {\n      \"type\": \"string\",\n      \"description\": \"Introductory price in micro-units of the currency.\"\n    },\n    \"introductoryPricePeriod\": {\n      \"type\": \"string\",\n      \"description\": \"Introductory price period in ISO 8601 format (e.g., P1W for one week, P1M for one month).\"\n    },\n    \"introductoryPriceCycles\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of billing periods the introductory price applies for.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-introductory-price-info-schema.json
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
title: IntroductoryPriceInfo
---
