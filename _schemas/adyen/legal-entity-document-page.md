---
description: DocumentPage schema from Adyen API
layout: schema
name: DocumentPage
properties_list:
- description: ''
  name: pageName
  type: string
- description: ''
  name: pageNumber
  type: integer
- description: ''
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-document-page-schema.json
slug: legal-entity-document-page
source_filename: legal-entity-document-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-document-page-schema.json\",\n  \"title\": \"DocumentPage\",\n  \"description\": \"DocumentPage schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pageName\": {\n      \"type\": \"string\"\n    },\n    \"pageNumber\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"type\": {\n      \"enum\": [\n        \"BACK\",\n        \"FRONT\",\n        \"UNDEFINED\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-document-page-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DocumentPage
---
