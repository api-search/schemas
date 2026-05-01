---
description: Details about a read set export job.
layout: schema
name: ExportReadSetJobDetail
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: sequenceStoreId
  type: object
- description: ''
  name: destination
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: completionTime
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-export-read-set-job-detail-schema.json
slug: healthomics-export-read-set-job-detail
source_filename: healthomics-export-read-set-job-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-job-detail-schema.json\",\n  \"title\": \"ExportReadSetJobDetail\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"sequenceStoreId\",\n    \"destination\",\n    \"status\",\n    \"creationTime\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportJobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    },\n    \"sequenceStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreId\"\n        },\n        {\n          \"description\": \"The job's sequence store ID.\"\n        }\n      ]\n    },\n    \"destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\
  \n        },\n        {\n          \"description\": \"The job's destination in Amazon S3.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetExportJobStatus\"\n        },\n        {\n          \"description\": \"The job's status.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the job was created.\"\n        }\n      ]\n    },\n    \"completionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the job completed.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Details about a read set export job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-export-read-set-job-detail-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ExportReadSetJobDetail
---
