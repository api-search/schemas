---
description: CapabilitySettings schema from Adyen API
layout: schema
name: CapabilitySettings
properties_list:
- description: The maximum amount a card holder can spend per industry.
  name: amountPerIndustry
  type: object
- description: The number of card holders who can use the card.
  name: authorizedCardUsers
  type: boolean
- description: The funding source of the card, for example **debit**.
  name: fundingSource
  type: array
- description: The period when the rule conditions apply.
  name: interval
  type: string
- description: The maximum amount a card holder can withdraw per day.
  name: maxAmount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-capability-settings-schema.json
slug: legal-entity-capability-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-capability-settings-schema.json\",\n  \"title\": \"CapabilitySettings\",\n  \"description\": \"CapabilitySettings schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amountPerIndustry\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/Amount\"\n      },\n      \"description\": \"The maximum amount a card holder can spend per industry.\",\n      \"type\": \"object\"\n    },\n    \"authorizedCardUsers\": {\n      \"description\": \"The number of card holders who can use the card.\",\n      \"type\": \"boolean\"\n    },\n    \"fundingSource\": {\n      \"description\": \"The funding source of the card, for example **debit**.\",\n      \"items\": {\n        \"enum\": [\n          \"credit\",\n          \"debit\",\n          \"prepaid\"\n        ],\n\
  \        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"interval\": {\n      \"description\": \"The period when the rule conditions apply.\",\n      \"enum\": [\n        \"daily\",\n        \"monthly\",\n        \"weekly\"\n      ],\n      \"type\": \"string\"\n    },\n    \"maxAmount\": {\n      \"description\": \"The maximum amount a card holder can withdraw per day.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-capability-settings-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CapabilitySettings
---
