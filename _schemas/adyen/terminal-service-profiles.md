---
description: ServiceProfiles schema from Adyen API
layout: schema
name: ServiceProfiles
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-service-profiles-schema.json
slug: terminal-service-profiles
source_filename: terminal-service-profiles-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-service-profiles-schema.json\",\n  \"title\": \"ServiceProfiles\",\n  \"description\": \"ServiceProfiles schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"Batch\",\n      \"CardReader\",\n      \"Communication\",\n      \"Loyalty\",\n      \"OneTimeRes\",\n      \"PIN\",\n      \"Reservation\",\n      \"Sound\",\n      \"StoredValue\",\n      \"Synchro\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-service-profiles-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ServiceProfiles
---
