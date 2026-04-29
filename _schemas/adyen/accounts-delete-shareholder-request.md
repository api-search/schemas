---
description: DeleteShareholderRequest schema from Adyen API
layout: schema
name: DeleteShareholderRequest
properties_list:
- description: The code of the Account Holder from which to delete the Shareholders.
  name: accountHolderCode
  type: string
- description: The code(s) of the Shareholders to be deleted.
  name: shareholderCodes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-delete-shareholder-request-schema.json
slug: accounts-delete-shareholder-request
source_filename: accounts-delete-shareholder-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-shareholder-request-schema.json\",\n  \"title\": \"DeleteShareholderRequest\",\n  \"description\": \"DeleteShareholderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder from which to delete the Shareholders.\",\n      \"type\": \"string\"\n    },\n    \"shareholderCodes\": {\n      \"description\": \"The code(s) of the Shareholders to be deleted.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"shareholderCodes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-shareholder-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeleteShareholderRequest
---
