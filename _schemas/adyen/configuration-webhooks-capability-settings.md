---
description: CapabilitySettings schema from Adyen API
layout: schema
name: CapabilitySettings
properties_list:
- description: ''
  name: amountPerIndustry
  type: object
- description: ''
  name: authorizedCardUsers
  type: boolean
- description: ''
  name: fundingSource
  type: array
- description: ''
  name: interval
  type: string
- description: ''
  name: maxAmount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-capability-settings-schema.json
slug: configuration-webhooks-capability-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-capability-settings-schema.json\",\n  \"title\": \"CapabilitySettings\",\n  \"description\": \"CapabilitySettings schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amountPerIndustry\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/Amount\"\n      },\n      \"description\": \"\",\n      \"type\": \"object\"\n    },\n    \"authorizedCardUsers\": {\n      \"description\": \"\",\n      \"type\": \"boolean\"\n    },\n    \"fundingSource\": {\n      \"description\": \"\",\n      \"items\": {\n        \"enum\": [\n          \"credit\",\n          \"debit\",\n          \"prepaid\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"interval\": {\n      \"description\": \"\",\n      \"enum\": [\n\
  \        \"daily\",\n        \"monthly\",\n        \"weekly\"\n      ],\n      \"type\": \"string\"\n    },\n    \"maxAmount\": {\n      \"description\": \"\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-capability-settings-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapabilitySettings
---
