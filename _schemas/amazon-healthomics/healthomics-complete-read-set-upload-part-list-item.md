---
description: Part of the response to the CompleteReadSetUpload API, including metadata.
layout: schema
name: CompleteReadSetUploadPartListItem
properties_list:
- description: ''
  name: partNumber
  type: object
- description: ''
  name: partSource
  type: object
- description: ''
  name: checksum
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-complete-read-set-upload-part-list-item-schema.json
slug: healthomics-complete-read-set-upload-part-list-item
source_filename: healthomics-complete-read-set-upload-part-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-complete-read-set-upload-part-list-item-schema.json\",\n  \"title\": \"CompleteReadSetUploadPartListItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"partNumber\",\n    \"partSource\",\n    \"checksum\"\n  ],\n  \"properties\": {\n    \"partNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompleteReadSetUploadPartListItemPartNumberInteger\"\n        },\n        {\n          \"description\": \" A number identifying the part in a read set upload. \"\n        }\n      ]\n    },\n    \"partSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetPartSource\"\n        },\n        {\n          \"description\": \" The source file of the part being uploaded. \"\n        }\n      ]\n    },\n    \"checksum\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A unique identifier used to confirm that parts are being added to the correct upload. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" Part of the response to the CompleteReadSetUpload API, including metadata. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-complete-read-set-upload-part-list-item-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CompleteReadSetUploadPartListItem
---
