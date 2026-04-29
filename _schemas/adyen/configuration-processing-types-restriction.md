---
description: ProcessingTypesRestriction schema from Adyen API
layout: schema
name: ProcessingTypesRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: 'List of processing types. Possible values: **atmWithdraw**, **balanceInquiry**, **ecommerce**, **moto**, **pos**, **recurring**, **token**.'
  name: value
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-processing-types-restriction-schema.json
slug: configuration-processing-types-restriction
source_filename: configuration-processing-types-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-processing-types-restriction-schema.json\",\n  \"title\": \"ProcessingTypesRestriction\",\n  \"description\": \"ProcessingTypesRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of processing types.\\n\\nPossible values: **atmWithdraw**, **balanceInquiry**, **ecommerce**, **moto**, **pos**, **recurring**, **token**.\\n\\n\",\n      \"items\": {\n        \"enum\": [\n          \"atmWithdraw\",\n          \"balanceInquiry\",\n          \"ecommerce\",\n          \"moto\",\n          \"pos\",\n          \"recurring\",\n          \"token\",\n          \"unknown\"\n        ],\n        \"type\":\
  \ \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-processing-types-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ProcessingTypesRestriction
---
