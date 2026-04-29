---
description: ServicesEnabled schema from Adyen API
layout: schema
name: ServicesEnabled
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-services-enabled-schema.json
slug: terminal-services-enabled
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-services-enabled-schema.json\",\n  \"title\": \"ServicesEnabled\",\n  \"description\": \"ServicesEnabled schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"CardAcquisition\",\n      \"Loyalty\",\n      \"Payment\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-services-enabled-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ServicesEnabled
---
