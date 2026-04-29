---
description: AndroidAppsResponse schema from Adyen API
layout: schema
name: AndroidAppsResponse
properties_list:
- description: Apps uploaded for Android payment terminals.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-android-apps-response-schema.json
slug: management-android-apps-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-android-apps-response-schema.json\",\n  \"title\": \"AndroidAppsResponse\",\n  \"description\": \"AndroidAppsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"Apps uploaded for Android payment terminals.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AndroidApp\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-android-apps-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AndroidAppsResponse
---
