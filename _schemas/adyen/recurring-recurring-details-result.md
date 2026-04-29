---
description: RecurringDetailsResult schema from Adyen API
layout: schema
name: RecurringDetailsResult
properties_list:
- description: The date when the recurring details were created.
  name: creationDate
  type: string
- description: Payment details stored for recurring payments.
  name: details
  type: array
- description: The most recent email for this shopper (if available).
  name: lastKnownShopperEmail
  type: string
- description: The reference you use to uniquely identify the shopper (e.g. user ID or account ID).
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-recurring-details-result-schema.json
slug: recurring-recurring-details-result
source_filename: recurring-recurring-details-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-recurring-details-result-schema.json\",\n  \"title\": \"RecurringDetailsResult\",\n  \"description\": \"RecurringDetailsResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creationDate\": {\n      \"description\": \"The date when the recurring details were created.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"description\": \"Payment details stored for recurring payments.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RecurringDetailWrapper\"\n      },\n      \"type\": \"array\"\n    },\n    \"lastKnownShopperEmail\": {\n      \"description\": \"The most recent email for this shopper (if available).\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The\
  \ reference you use to uniquely identify the shopper (e.g. user ID or account ID).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-recurring-details-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RecurringDetailsResult
---
