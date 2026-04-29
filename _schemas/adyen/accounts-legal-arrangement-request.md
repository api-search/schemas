---
description: LegalArrangementRequest schema from Adyen API
layout: schema
name: LegalArrangementRequest
properties_list:
- description: The code of the legal arrangement to be deleted. If you also send `legalArrangementEntityCodes`, only the entities listed will be deleted.
  name: legalArrangementCode
  type: string
- description: List of legal arrangement entities to be deleted.
  name: legalArrangementEntityCodes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-legal-arrangement-request-schema.json
slug: accounts-legal-arrangement-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-legal-arrangement-request-schema.json\",\n  \"title\": \"LegalArrangementRequest\",\n  \"description\": \"LegalArrangementRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"legalArrangementCode\": {\n      \"description\": \"The code of the legal arrangement to be deleted. If you also send `legalArrangementEntityCodes`, only the entities listed will be deleted.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementEntityCodes\": {\n      \"description\": \"List of legal arrangement entities to be deleted.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"legalArrangementCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-legal-arrangement-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LegalArrangementRequest
---
