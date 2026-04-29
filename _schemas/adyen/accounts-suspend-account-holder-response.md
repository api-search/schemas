---
description: SuspendAccountHolderResponse schema from Adyen API
layout: schema
name: SuspendAccountHolderResponse
properties_list:
- description: The new status of the Account Holder.
  name: accountHolderStatus
  type: object
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-suspend-account-holder-response-schema.json
slug: accounts-suspend-account-holder-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-suspend-account-holder-response-schema.json\",\n  \"title\": \"SuspendAccountHolderResponse\",\n  \"description\": \"SuspendAccountHolderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderStatus\": {\n      \"description\": \"The new status of the Account Holder.\",\n      \"$ref\": \"#/components/schemas/AccountHolderStatus\"\n    },\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n\
  \      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-suspend-account-holder-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SuspendAccountHolderResponse
---
