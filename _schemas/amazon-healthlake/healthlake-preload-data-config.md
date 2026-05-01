---
description: The input properties for the preloaded data store. Only data preloaded from Synthea is supported.
layout: schema
name: PreloadDataConfig
properties_list:
- description: ''
  name: PreloadDataType
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-preload-data-config-schema.json
slug: healthlake-preload-data-config
source_filename: healthlake-preload-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-preload-data-config-schema.json\",\n  \"title\": \"PreloadDataConfig\",\n  \"type\": \"object\",\n  \"required\": [\n    \"PreloadDataType\"\n  ],\n  \"properties\": {\n    \"PreloadDataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PreloadDataType\"\n        },\n        {\n          \"description\": \"The type of preloaded data. Only Synthea preloaded data is supported.\"\n        }\n      ]\n    }\n  },\n  \"description\": \" The input properties for the preloaded data store. Only data preloaded from Synthea is supported.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-preload-data-config-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: PreloadDataConfig
---
