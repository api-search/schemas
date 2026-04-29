---
description: CloseAccountResponse schema from Adyen API
layout: schema
name: CloseAccountResponse
properties_list:
- description: The account code of the account that is closed.
  name: accountCode
  type: string
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
- description: 'The new status of the account. >Permitted values: `Active`, `Inactive`, `Suspended`, `Closed`.'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-close-account-response-schema.json
slug: notifications-close-account-response
source_filename: notifications-close-account-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-close-account-response-schema.json\",\n  \"title\": \"CloseAccountResponse\",\n  \"description\": \"CloseAccountResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"The account code of the account that is closed.\",\n      \"type\": \"string\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"\
  string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The new status of the account.\\n>Permitted values: `Active`, `Inactive`, `Suspended`, `Closed`.\",\n      \"enum\": [\n        \"Active\",\n        \"Closed\",\n        \"Inactive\",\n        \"Suspended\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-close-account-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CloseAccountResponse
---
