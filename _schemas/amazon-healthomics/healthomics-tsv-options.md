---
description: Formatting options for a TSV file.
layout: schema
name: TsvOptions
properties_list:
- description: ''
  name: readOptions
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-tsv-options-schema.json
slug: healthomics-tsv-options
source_filename: healthomics-tsv-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-tsv-options-schema.json\",\n  \"title\": \"TsvOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"readOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadOptions\"\n        },\n        {\n          \"description\": \"The file's read options.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Formatting options for a TSV file.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-tsv-options-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: TsvOptions
---
