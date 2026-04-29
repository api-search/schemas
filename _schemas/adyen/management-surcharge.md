---
description: Surcharge schema from Adyen API
layout: schema
name: Surcharge
properties_list:
- description: Show the surcharge details on the terminal, so the shopper can confirm.
  name: askConfirmation
  type: boolean
- description: Surcharge fees or percentages for specific payment methods, funding sources (credit or debit), and currencies.
  name: configurations
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-surcharge-schema.json
slug: management-surcharge
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-surcharge-schema.json\",\n  \"title\": \"Surcharge\",\n  \"description\": \"Surcharge schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"askConfirmation\": {\n      \"description\": \"Show the surcharge details on the terminal, so the shopper can confirm.\",\n      \"type\": \"boolean\"\n    },\n    \"configurations\": {\n      \"description\": \"Surcharge fees or percentages for specific payment methods, funding sources (credit or debit), and currencies.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Configuration\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-surcharge-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Surcharge
---
