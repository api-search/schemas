---
description: WifiProfiles schema from Adyen API
layout: schema
name: WifiProfiles
properties_list:
- description: List of remote Wi-Fi profiles.
  name: profiles
  type: array
- description: General Wi-Fi settings.
  name: settings
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-wifi-profiles-schema.json
slug: management-wifi-profiles
source_filename: management-wifi-profiles-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-wifi-profiles-schema.json\",\n  \"title\": \"WifiProfiles\",\n  \"description\": \"WifiProfiles schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profiles\": {\n      \"description\": \"List of remote Wi-Fi profiles.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Profile\"\n      },\n      \"type\": \"array\"\n    },\n    \"settings\": {\n      \"description\": \"General Wi-Fi settings.\",\n      \"$ref\": \"#/components/schemas/Settings\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-wifi-profiles-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: WifiProfiles
---
