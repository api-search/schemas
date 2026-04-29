---
description: An object containing <code>InputRecords</code>, <code>TotalRecordsProcessed</code>, <code>MatchIDs</code>, and <code>RecordsNotProcessed</code>.
layout: schema
name: JobMetrics
properties_list:
- description: ''
  name: inputRecords
  type: object
- description: ''
  name: matchIDs
  type: object
- description: ''
  name: recordsNotProcessed
  type: object
- description: ''
  name: totalRecordsProcessed
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-job-metrics-schema.json
slug: amazon-entity-resolution-job-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-job-metrics-schema.json\",\n  \"title\": \"JobMetrics\",\n  \"description\": \"An object containing <code>InputRecords</code>, <code>TotalRecordsProcessed</code>, <code>MatchIDs</code>, and <code>RecordsNotProcessed</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of input records.\"\n        }\n      ]\n    },\n    \"matchIDs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of <code>matchID</code>s generated.\"\n        }\n      ]\n    },\n    \"recordsNotProcessed\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of records that did not get processed,\"\n        }\n      ]\n    },\n    \"totalRecordsProcessed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The total number of records processed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-job-metrics-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: JobMetrics
---
