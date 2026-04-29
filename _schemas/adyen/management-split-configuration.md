---
description: SplitConfiguration schema from Adyen API
layout: schema
name: SplitConfiguration
properties_list:
- description: Your description for the split configuration.
  name: description
  type: string
- description: Array of rules that define the split configuration behavior.
  name: rules
  type: array
- description: Unique identifier of the split configuration.
  name: splitConfigurationId
  type: string
- description: List of stores to which the split configuration applies.
  name: stores
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-split-configuration-schema.json
slug: management-split-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-split-configuration-schema.json\",\n  \"title\": \"SplitConfiguration\",\n  \"description\": \"SplitConfiguration schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"Your description for the split configuration.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"rules\": {\n      \"description\": \"Array of rules that define the split configuration behavior.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SplitConfigurationRule\"\n      },\n      \"type\": \"array\"\n    },\n    \"splitConfigurationId\": {\n      \"description\": \"Unique identifier of the split configuration.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"stores\": {\n      \"description\": \"List of stores\
  \ to which the split configuration applies.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"description\",\n    \"rules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-split-configuration-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SplitConfiguration
---
