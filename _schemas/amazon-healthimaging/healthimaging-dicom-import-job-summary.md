---
description: Summary of import job.
layout: schema
name: DICOMImportJobSummary
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: jobName
  type: object
- description: ''
  name: jobStatus
  type: object
- description: ''
  name: datastoreId
  type: object
- description: ''
  name: dataAccessRoleArn
  type: object
- description: ''
  name: endedAt
  type: object
- description: ''
  name: submittedAt
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon HealthImaging
provider_slug: amazon-healthimaging
schema_file: json-schema/healthimaging-dicom-import-job-summary-schema.json
slug: healthimaging-dicom-import-job-summary
source_filename: healthimaging-dicom-import-job-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-import-job-summary-schema.json\",\n  \"title\": \"DICOMImportJobSummary\",\n  \"type\": \"object\",\n  \"required\": [\n    \"jobId\",\n    \"jobName\",\n    \"jobStatus\",\n    \"datastoreId\"\n  ],\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The import job identifier.\"\n        }\n      ]\n    },\n    \"jobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The import job name.\"\n        }\n      ]\n    },\n    \"jobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\"\
  : \"The filters for listing import jobs based on status.\"\n        }\n      ]\n    },\n    \"datastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The data store identifier.\"\n        }\n      ]\n    },\n    \"dataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that grants permissions to access medical imaging resources.\"\n        }\n      ]\n    },\n    \"endedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when an import job ended.\"\n        }\n      ]\n    },\n    \"submittedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp when\
  \ an import job was submitted.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The error message thrown if an import job fails.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Summary of import job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthimaging/refs/heads/main/json-schema/healthimaging-dicom-import-job-summary-schema.json
tags:
- Healthcare
- HIPAA
- Machine Learning
- Medical Imaging
- DICOM
title: DICOMImportJobSummary
---
