---
description: Gratuity schema from Adyen API
layout: schema
name: Gratuity
properties_list:
- description: Indicates whether one of the predefined tipping options is to let the shopper enter a custom tip. If **true**, only three of the other options defined in `predefinedTipEntries` are shown.
  name: allowCustomAmount
  type: boolean
- description: The currency that the tipping settings apply to.
  name: currency
  type: string
- description: 'Tipping options the shopper can choose from if `usePredefinedTipEntries` is **true**. The maximum number of predefined options is four, or three plus the option to enter a custom tip. The options can '
  name: predefinedTipEntries
  type: array
- description: Indicates whether the terminal shows a prompt to enter a tip (**false**), or predefined tipping options to choose from (**true**).
  name: usePredefinedTipEntries
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-gratuity-schema.json
slug: management-gratuity
source_filename: management-gratuity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-gratuity-schema.json\",\n  \"title\": \"Gratuity\",\n  \"description\": \"Gratuity schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowCustomAmount\": {\n      \"description\": \"Indicates whether one of the predefined tipping options is to let the shopper enter a custom tip. If **true**, only three of the other options defined in `predefinedTipEntries` are shown.\",\n      \"type\": \"boolean\"\n    },\n    \"currency\": {\n      \"description\": \"The currency that the tipping settings apply to.\",\n      \"type\": \"string\"\n    },\n    \"predefinedTipEntries\": {\n      \"description\": \"Tipping options the shopper can choose from if `usePredefinedTipEntries` is **true**. The maximum number of predefined options is four, or three plus the option to enter a custom tip.\\\
  nThe options can be a mix of:\\n\\n- A percentage of the transaction amount. Example: **5%**\\n- A tip amount in [minor units](https://docs.adyen.com/development-resources/currency-codes). Example: **500** for a EUR 5 tip.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"usePredefinedTipEntries\": {\n      \"description\": \"Indicates whether the terminal shows a prompt to enter a tip (**false**), or predefined tipping options to choose from (**true**).\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-gratuity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Gratuity
---
