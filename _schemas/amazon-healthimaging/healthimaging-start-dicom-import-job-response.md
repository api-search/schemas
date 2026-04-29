---
description: ''
layout: schema
name: StartDICOMImportJobResponse
properties_list:
- description: ''
  name: datastoreId
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: jobStatus
  type: object
- description: ''
  name: submittedAt
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-start-dicom-import-job-response-schema.json
slug: healthimaging-start-dicom-import-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-start-dicom-import-job-response-schema.json\",\n  \"title\": \"StartDICOMImportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"datastoreId\",\n    \"jobId\",\n    \"jobStatus\",\n    \"submittedAt\"\n  ],\n  \"properties\": {\n    \"datastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The data store identifier.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The import job identifier.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n     \
  \   },\n        {\n          \"description\": \"The import job status.\"\n        }\n      ]\n    },\n    \"submittedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when the import job was submitted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-start-dicom-import-job-response-schema.json
tags:
- AWS
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: StartDICOMImportJobResponse
---
