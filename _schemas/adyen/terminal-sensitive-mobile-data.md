---
description: SensitiveMobileData schema from Adyen API
layout: schema
name: SensitiveMobileData
properties_list:
- description: ''
  name: MSISDN
  type: integer
- description: ''
  name: ISMI
  type: integer
- description: ''
  name: IMEI
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sensitive-mobile-data-schema.json
slug: terminal-sensitive-mobile-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sensitive-mobile-data-schema.json\",\n  \"title\": \"SensitiveMobileData\",\n  \"description\": \"SensitiveMobileData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MSISDN\": {\n      \"type\": \"integer\"\n    },\n    \"ISMI\": {\n      \"type\": \"integer\"\n    },\n    \"IMEI\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"MSISDN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sensitive-mobile-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SensitiveMobileData
---
