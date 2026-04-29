---
description: ViasPersonalData schema from Adyen API
layout: schema
name: ViasPersonalData
properties_list:
- description: The person's date of birth, in ISO-8601 YYYY-MM-DD format. For example, **2000-01-31**.
  name: dateOfBirth
  type: string
- description: Array that contains information about the person's identification document. You can submit only one entry per document type.
  name: documentData
  type: array
- description: The nationality of the person represented by a two-character country code, in [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) format. For example, **NL**.
  name: nationality
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-vias-personal-data-schema.json
slug: notifications-vias-personal-data
source_filename: notifications-vias-personal-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-vias-personal-data-schema.json\",\n  \"title\": \"ViasPersonalData\",\n  \"description\": \"ViasPersonalData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dateOfBirth\": {\n      \"description\": \"The person's date of birth, in ISO-8601 YYYY-MM-DD format. For example, **2000-01-31**.\",\n      \"type\": \"string\"\n    },\n    \"documentData\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"Array that contains information about the person's identification document. You can submit only one entry per document type.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PersonalDocumentData\"\n      },\n      \"type\": \"array\"\n    },\n    \"nationality\": {\n      \"description\": \"The nationality of the person represented by a two-character\
  \ country code,  in [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) format. For example, **NL**.\\n\",\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-vias-personal-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ViasPersonalData
---
