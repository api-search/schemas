---
description: Formatting options for a file.
layout: schema
name: FormatOptions
properties_list:
- description: ''
  name: tsvOptions
  type: object
- description: ''
  name: vcfOptions
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-format-options-schema.json
slug: healthomics-format-options
source_filename: healthomics-format-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-format-options-schema.json\",\n  \"title\": \"FormatOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tsvOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TsvOptions\"\n        },\n        {\n          \"description\": \"Options for a TSV file.\"\n        }\n      ]\n    },\n    \"vcfOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VcfOptions\"\n        },\n        {\n          \"description\": \"Options for a VCF file.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Formatting options for a file.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-format-options-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: FormatOptions
---
