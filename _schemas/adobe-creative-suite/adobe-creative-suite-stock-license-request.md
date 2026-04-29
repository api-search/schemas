---
description: Request body for licensing a stock asset
layout: schema
name: LicenseRequest
properties_list:
- description: Adobe Stock content ID of the asset to license
  name: content_id
  type: integer
- description: License type to apply
  name: license
  type: string
- description: BCP 47 locale for localized response data
  name: locale
  type: string
- description: Optional purchase parameters and reference metadata
  name: purchase_params
  type: object
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-license-request-schema.json
slug: adobe-creative-suite-stock-license-request
source_filename: adobe-creative-suite-stock-license-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-request-schema.json\",\n  \"title\": \"LicenseRequest\",\n  \"description\": \"Request body for licensing a stock asset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Adobe Stock content ID of the asset to license\",\n      \"example\": 123456789\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"License type to apply\",\n      \"enum\": [\n        \"Standard\",\n        \"Extended\",\n        \"Video_HD\",\n        \"Video_4K\"\n      ],\n      \"example\": \"Standard\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"BCP 47 locale for localized response data\",\n      \"example\": \"en_US\"\n    },\n    \"purchase_params\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Optional purchase parameters and reference metadata\",\n      \"properties\": {\n        \"references\": {\n          \"type\": \"array\",\n          \"description\": \"List of reference key-value pairs for tracking the license\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/LicenseReference\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"content_id\",\n    \"license\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-request-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: LicenseRequest
---
