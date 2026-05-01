---
description: A read set.
layout: schema
name: ExportReadSet
properties_list:
- description: ''
  name: readSetId
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-export-read-set-schema.json
slug: healthomics-export-read-set
source_filename: healthomics-export-read-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-schema.json\",\n  \"title\": \"ExportReadSet\",\n  \"type\": \"object\",\n  \"required\": [\n    \"readSetId\"\n  ],\n  \"properties\": {\n    \"readSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetId\"\n        },\n        {\n          \"description\": \"The set's ID.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A read set.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ExportReadSet
---
