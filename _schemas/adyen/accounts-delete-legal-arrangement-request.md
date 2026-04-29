---
description: DeleteLegalArrangementRequest schema from Adyen API
layout: schema
name: DeleteLegalArrangementRequest
properties_list:
- description: The code of the account holder.
  name: accountHolderCode
  type: string
- description: List of legal arrangements.
  name: legalArrangements
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-delete-legal-arrangement-request-schema.json
slug: accounts-delete-legal-arrangement-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-legal-arrangement-request-schema.json\",\n  \"title\": \"DeleteLegalArrangementRequest\",\n  \"description\": \"DeleteLegalArrangementRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"description\": \"The code of the account holder.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangements\": {\n      \"description\": \"List of legal arrangements.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LegalArrangementRequest\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"legalArrangements\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-delete-legal-arrangement-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DeleteLegalArrangementRequest
---
