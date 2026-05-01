---
description: ''
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-tag-resource-request-schema.json
slug: healthomics-tag-resource-request
source_filename: healthomics-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"tags\"\n  ],\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagResourceRequestTagsMap\"\n        },\n        {\n          \"description\": \"Tags for the resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-tag-resource-request-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: TagResourceRequest
---
