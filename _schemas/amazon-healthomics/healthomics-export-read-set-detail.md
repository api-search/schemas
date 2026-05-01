---
description: Details about a read set.
layout: schema
name: ExportReadSetDetail
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusMessage
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-export-read-set-detail-schema.json
slug: healthomics-export-read-set-detail
source_filename: healthomics-export-read-set-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-detail-schema.json\",\n  \"title\": \"ExportReadSetDetail\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetId\"\n        },\n        {\n          \"description\": \"The set's ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetExportJobItemStatus\"\n        },\n        {\n          \"description\": \"The set's status.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatusMessage\"\n        },\n        {\n          \"description\": \"The set's status message.\"\
  \n        }\n      ]\n    }\n  },\n  \"description\": \"Details about a read set.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-detail-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ExportReadSetDetail
---
