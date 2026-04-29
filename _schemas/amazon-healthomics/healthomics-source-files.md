---
description: Source files for a sequence.
layout: schema
name: SourceFiles
properties_list:
- description: ''
  name: source1
  type: object
- description: ''
  name: source2
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-source-files-schema.json
slug: healthomics-source-files
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-source-files-schema.json\",\n  \"title\": \"SourceFiles\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source1\"\n  ],\n  \"properties\": {\n    \"source1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The location of the first file in Amazon S3.\"\n        }\n      ]\n    },\n    \"source2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The location of the second file in Amazon S3.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Source files for a sequence.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-source-files-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: SourceFiles
---
