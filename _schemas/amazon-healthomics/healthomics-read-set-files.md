---
description: Files in a read set.
layout: schema
name: ReadSetFiles
properties_list:
- description: ''
  name: source1
  type: object
- description: ''
  name: source2
  type: object
- description: ''
  name: index
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-read-set-files-schema.json
slug: healthomics-read-set-files
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-files-schema.json\",\n  \"title\": \"ReadSetFiles\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformation\"\n        },\n        {\n          \"description\": \"The location of the first file in Amazon S3.\"\n        }\n      ]\n    },\n    \"source2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformation\"\n        },\n        {\n          \"description\": \"The location of the second file in Amazon S3.\"\n        }\n      ]\n    },\n    \"index\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformation\"\n        },\n        {\n          \"description\": \"The files' index.\"\n        }\n      ]\n \
  \   }\n  },\n  \"description\": \"Files in a read set.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-files-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReadSetFiles
---
