---
description: An genome reference source.
layout: schema
name: ImportReferenceSourceItem
properties_list:
- description: ''
  name: sourceFile
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
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
schema_file: json-schema/healthomics-import-reference-source-item-schema.json
slug: healthomics-import-reference-source-item
source_filename: healthomics-import-reference-source-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-import-reference-source-item-schema.json\",\n  \"title\": \"ImportReferenceSourceItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"status\"\n  ],\n  \"properties\": {\n    \"sourceFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The source file's location in Amazon S3.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceImportJobItemStatus\"\n        },\n        {\n          \"description\": \"The source's status.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatusMessage\"\n        },\n        {\n          \"description\"\
  : \"The source's status message.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceName\"\n        },\n        {\n          \"description\": \"The source's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceDescription\"\n        },\n        {\n          \"description\": \"The source's description.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The source's tags.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An genome reference source.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-import-reference-source-item-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ImportReferenceSourceItem
---
