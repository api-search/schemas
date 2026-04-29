---
description: Represents a monetary amount with currency.
layout: schema
name: Money
properties_list:
- description: ISO 4217 three-letter currency code (e.g., USD, EUR).
  name: currencyCode
  type: string
- description: The whole units of the amount.
  name: units
  type: string
- description: Number of nano units (10^-9) of the amount. Must be between -999,999,999 and +999,999,999.
  name: nanos
  type: integer
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-money-schema.json
slug: google-play-developer-money
source_filename: google-play-developer-money-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Money\",\n  \"type\": \"object\",\n  \"description\": \"Represents a monetary amount with currency.\",\n  \"properties\": {\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code (e.g., USD, EUR).\"\n    },\n    \"units\": {\n      \"type\": \"string\",\n      \"description\": \"The whole units of the amount.\"\n    },\n    \"nanos\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of nano units (10^-9) of the amount. Must be between -999,999,999 and +999,999,999.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-money-schema.json
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
title: Money
---
