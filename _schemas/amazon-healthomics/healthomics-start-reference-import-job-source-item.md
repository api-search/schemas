---
description: A source for a reference import job.
layout: schema
name: StartReferenceImportJobSourceItem
properties_list:
- description: ''
  name: sourceFile
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-start-reference-import-job-source-item-schema.json
slug: healthomics-start-reference-import-job-source-item
source_filename: healthomics-start-reference-import-job-source-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-reference-import-job-source-item-schema.json\",\n  \"title\": \"StartReferenceImportJobSourceItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sourceFile\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"sourceFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The source file's location in Amazon S3.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceName\"\n        },\n        {\n          \"description\": \"The source's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceDescription\"\n        },\n        {\n\
  \          \"description\": \"The source's description.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The source's tags.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A source for a reference import job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-reference-import-job-source-item-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: StartReferenceImportJobSourceItem
---
