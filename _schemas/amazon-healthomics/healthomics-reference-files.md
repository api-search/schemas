---
description: A set of genome reference files.
layout: schema
name: ReferenceFiles
properties_list:
- description: ''
  name: source
  type: object
- description: ''
  name: index
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-reference-files-schema.json
slug: healthomics-reference-files
source_filename: healthomics-reference-files-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-reference-files-schema.json\",\n  \"title\": \"ReferenceFiles\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformation\"\n        },\n        {\n          \"description\": \"The source file's location in Amazon S3.\"\n        }\n      ]\n    },\n    \"index\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformation\"\n        },\n        {\n          \"description\": \"The files' index.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A set of genome reference files.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-reference-files-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReferenceFiles
---
