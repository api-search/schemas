---
description: DefenseDocument schema from Adyen API
layout: schema
name: DefenseDocument
properties_list:
- description: The content of the defense document.
  name: content
  type: string
- description: The content type of the defense document.
  name: contentType
  type: string
- description: The document type code of the defense document.
  name: defenseDocumentTypeCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/disputes-defense-document-schema.json
slug: disputes-defense-document
source_filename: disputes-defense-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-document-schema.json\",\n  \"title\": \"DefenseDocument\",\n  \"description\": \"DefenseDocument schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The content of the defense document.\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"contentType\": {\n      \"description\": \"The content type of the defense document.\",\n      \"type\": \"string\"\n    },\n    \"defenseDocumentTypeCode\": {\n      \"description\": \"The document type code of the defense document.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"defenseDocumentTypeCode\",\n    \"contentType\",\n    \"content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/disputes-defense-document-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DefenseDocument
---
