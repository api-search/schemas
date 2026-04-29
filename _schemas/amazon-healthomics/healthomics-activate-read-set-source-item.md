---
description: A source for a read set activation job.
layout: schema
name: ActivateReadSetSourceItem
properties_list:
- description: ''
  name: readSetId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-activate-read-set-source-item-schema.json
slug: healthomics-activate-read-set-source-item
source_filename: healthomics-activate-read-set-source-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-activate-read-set-source-item-schema.json\",\n  \"title\": \"ActivateReadSetSourceItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"readSetId\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"readSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetId\"\n        },\n        {\n          \"description\": \"The source's read set ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetActivationJobItemStatus\"\n        },\n        {\n          \"description\": \"The source's status.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatusMessage\"\n        },\n        {\n       \
  \   \"description\": \"The source's status message.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A source for a read set activation job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-activate-read-set-source-item-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ActivateReadSetSourceItem
---
