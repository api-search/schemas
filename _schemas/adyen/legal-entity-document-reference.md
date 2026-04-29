---
description: DocumentReference schema from Adyen API
layout: schema
name: DocumentReference
properties_list:
- description: Identifies whether the document is active and used for checks.
  name: active
  type: boolean
- description: Your description for the document.
  name: description
  type: string
- description: Document name.
  name: fileName
  type: string
- description: The unique identifier of the resource.
  name: id
  type: string
- description: The modification date of the document.
  name: modificationDate
  type: string
- description: List of document pages
  name: pages
  type: array
- description: Type of document, used when providing an ID number or uploading a document.
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-document-reference-schema.json
slug: legal-entity-document-reference
source_filename: legal-entity-document-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-document-reference-schema.json\",\n  \"title\": \"DocumentReference\",\n  \"description\": \"DocumentReference schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"active\": {\n      \"description\": \"Identifies whether the document is active and used for checks.\",\n      \"type\": \"boolean\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the document.\",\n      \"type\": \"string\"\n    },\n    \"fileName\": {\n      \"description\": \"Document name.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the resource.\",\n      \"type\": \"string\"\n    },\n    \"modificationDate\": {\n      \"description\": \"The modification date of the document.\",\n      \"format\": \"date-time\",\n   \
  \   \"type\": \"string\"\n    },\n    \"pages\": {\n      \"description\": \"List of document pages\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DocumentPage\"\n      },\n      \"type\": \"array\"\n    },\n    \"type\": {\n      \"description\": \"Type of document, used when providing an ID number or uploading a document.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-document-reference-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DocumentReference
---
