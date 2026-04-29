---
description: PayoutSettingsResponse schema from Adyen API
layout: schema
name: PayoutSettingsResponse
properties_list:
- description: The list of payout accounts.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-payout-settings-response-schema.json
slug: management-payout-settings-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payout-settings-response-schema.json\",\n  \"title\": \"PayoutSettingsResponse\",\n  \"description\": \"PayoutSettingsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"The list of payout accounts.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PayoutSettings\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-payout-settings-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PayoutSettingsResponse
---
