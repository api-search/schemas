---
description: Formatting options for a VCF file.
layout: schema
name: VcfOptions
properties_list:
- description: ''
  name: ignoreQualField
  type: object
- description: ''
  name: ignoreFilterField
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-vcf-options-schema.json
slug: healthomics-vcf-options
source_filename: healthomics-vcf-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-vcf-options-schema.json\",\n  \"title\": \"VcfOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ignoreQualField\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The file's ignore qual field setting.\"\n        }\n      ]\n    },\n    \"ignoreFilterField\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The file's ignore filter field setting.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Formatting options for a VCF file.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-vcf-options-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: VcfOptions
---
