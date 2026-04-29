---
description: ''
layout: schema
name: ContactEnrichRequest
properties_list:
- description: ''
  name: outputFields
  type: array
- description: ''
  name: matchPersonInput
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-contact-enrich-request-schema.json
slug: zoominfo-contact-enrich-request
source_filename: zoominfo-contact-enrich-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"matchPersonInput\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"personId\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          }\n        },\n        \"required\": [\n          \"personId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"outputFields\",\n    \"matchPersonInput\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactEnrichRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-contact-enrich-request-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: ContactEnrichRequest
---
