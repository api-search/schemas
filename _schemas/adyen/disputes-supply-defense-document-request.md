---
description: SupplyDefenseDocumentRequest schema from Adyen API
layout: schema
name: SupplyDefenseDocumentRequest
properties_list:
- description: An array containing a list of the defense documents.
  name: defenseDocuments
  type: array
- description: The PSP reference assigned to the dispute.
  name: disputePspReference
  type: string
- description: The merchant account identifier, for which you want to process the dispute transaction.
  name: merchantAccountCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-supply-defense-document-request-schema.json
slug: disputes-supply-defense-document-request
source_filename: disputes-supply-defense-document-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-supply-defense-document-request-schema.json\",\n  \"title\": \"SupplyDefenseDocumentRequest\",\n  \"description\": \"SupplyDefenseDocumentRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defenseDocuments\": {\n      \"description\": \"An array containing a list of the defense documents.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DefenseDocument\"\n      },\n      \"type\": \"array\"\n    },\n    \"disputePspReference\": {\n      \"description\": \"The PSP reference assigned to the dispute.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccountCode\": {\n      \"description\": \"The merchant account identifier, for which you want to process the dispute transaction.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccountCode\"\
  ,\n    \"disputePspReference\",\n    \"defenseDocuments\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-supply-defense-document-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SupplyDefenseDocumentRequest
---
