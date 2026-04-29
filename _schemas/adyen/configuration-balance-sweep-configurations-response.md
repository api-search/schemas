---
description: BalanceSweepConfigurationsResponse schema from Adyen API
layout: schema
name: BalanceSweepConfigurationsResponse
properties_list:
- description: Indicates whether there are more items on the next page.
  name: hasNext
  type: boolean
- description: Indicates whether there are more items on the previous page.
  name: hasPrevious
  type: boolean
- description: List of sweeps associated with the balance account.
  name: sweeps
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-balance-sweep-configurations-response-schema.json
slug: configuration-balance-sweep-configurations-response
source_filename: configuration-balance-sweep-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-sweep-configurations-response-schema.json\",\n  \"title\": \"BalanceSweepConfigurationsResponse\",\n  \"description\": \"BalanceSweepConfigurationsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hasNext\": {\n      \"description\": \"Indicates whether there are more items on the next page.\",\n      \"type\": \"boolean\"\n    },\n    \"hasPrevious\": {\n      \"description\": \"Indicates whether there are more items on the previous page.\",\n      \"type\": \"boolean\"\n    },\n    \"sweeps\": {\n      \"description\": \"List of sweeps associated with the balance account.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SweepConfigurationV2\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"sweeps\",\n    \"hasPrevious\"\
  ,\n    \"hasNext\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-balance-sweep-configurations-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceSweepConfigurationsResponse
---
