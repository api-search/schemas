---
description: Settings schema from Adyen API
layout: schema
name: Settings
properties_list:
- description: 'The preferred Wi-Fi band, for use if the terminals support multiple bands. Possible values: All, 2.4GHz, 5GHz.'
  name: band
  type: string
- description: Indicates whether roaming is enabled on the terminals.
  name: roaming
  type: boolean
- description: 'The connection time-out in seconds. Minimum value: 0.'
  name: timeout
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-settings-schema.json
slug: management-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-settings-schema.json\",\n  \"title\": \"Settings\",\n  \"description\": \"Settings schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"band\": {\n      \"description\": \"The preferred Wi-Fi band, for use if the terminals support multiple bands. Possible values: All, 2.4GHz, 5GHz.\",\n      \"type\": \"string\"\n    },\n    \"roaming\": {\n      \"description\": \"Indicates whether roaming is enabled on the terminals.\",\n      \"type\": \"boolean\"\n    },\n    \"timeout\": {\n      \"description\": \"The connection time-out in seconds. Minimum value: 0.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-settings-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Settings
---
