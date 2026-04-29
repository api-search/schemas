---
description: AmountAdjustment schema from Adyen API
layout: schema
name: AmountAdjustment
properties_list:
- description: The adjustment amount.
  name: amount
  type: object
- description: 'The type of markup that is applied to an authorised payment. Possible values: **exchange**, **forexMarkup**, **authHoldReserve**, **atmMarkup**.'
  name: amountAdjustmentType
  type: string
- description: The basepoints associated with the applied markup.
  name: basepoints
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-amount-adjustment-schema.json
slug: transfer-webhooks-amount-adjustment
source_filename: transfer-webhooks-amount-adjustment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-amount-adjustment-schema.json\",\n  \"title\": \"AmountAdjustment\",\n  \"description\": \"AmountAdjustment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The adjustment amount.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"amountAdjustmentType\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of markup that is applied to an authorised payment.\\n\\nPossible values: **exchange**, **forexMarkup**, **authHoldReserve**, **atmMarkup**.\",\n      \"enum\": [\n        \"atmMarkup\",\n        \"authHoldReserve\",\n        \"exchange\",\n        \"forexMarkup\"\n      ],\n      \"type\": \"string\"\n    },\n    \"basepoints\": {\n      \"x-addedInVersion\"\
  : \"3\",\n      \"description\": \"The basepoints associated with the applied markup.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-amount-adjustment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AmountAdjustment
---
