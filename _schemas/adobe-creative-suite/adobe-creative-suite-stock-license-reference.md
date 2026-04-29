---
description: Optional purchase reference metadata for a license transaction
layout: schema
name: LicenseReference
properties_list:
- description: Reference ID provided by the API caller for tracking
  name: id
  type: integer
- description: Reference value such as a project name or purchase order number
  name: value
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-license-reference-schema.json
slug: adobe-creative-suite-stock-license-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-reference-schema.json\",\n  \"title\": \"LicenseReference\",\n  \"description\": \"Optional purchase reference metadata for a license transaction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Reference ID provided by the API caller for tracking\",\n      \"example\": 1001\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Reference value such as a project name or purchase order number\",\n      \"example\": \"Project Alpha\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-license-reference-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: LicenseReference
---
