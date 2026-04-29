---
description: DisableRequest schema from Adyen API
layout: schema
name: DisableRequest
properties_list:
- description: 'Specify the contract if you only want to disable a specific use. This field can be set to one of the following values, or to their combination (comma-separated): * ONECLICK * RECURRING * PAYOUT'
  name: contract
  type: string
- description: The merchant account identifier with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The ID that uniquely identifies the recurring detail reference. If it is not provided, the whole recurring contract of the `shopperReference` will be disabled, which includes all recurring details.
  name: recurringDetailReference
  type: string
- description: The ID that uniquely identifies the shopper. This `shopperReference` must be the same as the `shopperReference` used in the initial payment.
  name: shopperReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/recurring-disable-request-schema.json
slug: recurring-disable-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-request-schema.json\",\n  \"title\": \"DisableRequest\",\n  \"description\": \"DisableRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contract\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Specify the contract if you only want to disable a specific use.\\n\\nThis field can be set to one of the following values, or to their combination (comma-separated):\\n* ONECLICK\\n* RECURRING\\n* PAYOUT\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"The ID that uniquely identifies the recurring detail reference.\\n\\nIf it is\
  \ not provided, the whole recurring contract of the `shopperReference` will be disabled, which includes all recurring details.\",\n      \"type\": \"string\"\n    },\n    \"shopperReference\": {\n      \"description\": \"The ID that uniquely identifies the shopper.\\n\\nThis `shopperReference` must be the same as the `shopperReference` used in the initial payment.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"shopperReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/recurring-disable-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisableRequest
---
