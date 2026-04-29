---
description: DeleteSignatoriesRequest schema from Adyen API
layout: schema
name: DeleteSignatoriesRequest
properties_list:
- description: The code of the account holder from which to delete the signatories.
  name: accountHolderCode
  type: string
- description: Array of codes of the signatories to be deleted.
  name: signatoryCodes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-delete-signatories-request-schema.json
slug: accounts-delete-signatories-request
source_filename: accounts-delete-signatories-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-signatories-request-schema.json\",\n  \"title\": \"DeleteSignatoriesRequest\",\n  \"description\": \"DeleteSignatoriesRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder from which to delete the signatories.\",\n      \"type\": \"string\"\n    },\n    \"signatoryCodes\": {\n      \"description\": \"Array of codes of the signatories to be deleted.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"signatoryCodes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-signatories-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeleteSignatoriesRequest
---
