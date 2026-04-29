---
description: DefenseReason schema from Adyen API
layout: schema
name: DefenseReason
properties_list:
- description: Array of defense document types for a specific defense reason. Indicates the document types that you can submit to the schemes to defend this dispute, and whether they are required.
  name: defenseDocumentTypes
  type: array
- description: The defense reason code that was selected to defend this dispute.
  name: defenseReasonCode
  type: string
- description: Indicates if sufficient defense material has been supplied.
  name: satisfied
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-defense-reason-schema.json
slug: disputes-defense-reason
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-reason-schema.json\",\n  \"title\": \"DefenseReason\",\n  \"description\": \"DefenseReason schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defenseDocumentTypes\": {\n      \"description\": \"Array of defense document types for a specific defense reason. Indicates the document types that you can submit to the schemes to defend this dispute, and whether they are required.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DefenseDocumentType\"\n      },\n      \"type\": \"array\"\n    },\n    \"defenseReasonCode\": {\n      \"description\": \"The defense reason code that was selected to defend this dispute.\",\n      \"type\": \"string\"\n    },\n    \"satisfied\": {\n      \"description\": \"Indicates if sufficient defense material has been supplied.\"\
  ,\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"defenseReasonCode\",\n    \"satisfied\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-reason-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DefenseReason
---
