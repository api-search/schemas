---
description: The properties of a FHIR export job, including the ID, ARN, name, and the status of the job.
layout: schema
name: ExportJobProperties
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: SubmitTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-export-job-properties-schema.json
slug: healthlake-export-job-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-export-job-properties-schema.json\",\n  \"title\": \"ExportJobProperties\",\n  \"type\": \"object\",\n  \"required\": [\n    \"JobId\",\n    \"JobStatus\",\n    \"SubmitTime\",\n    \"DatastoreId\",\n    \"OutputDataConfig\"\n  ],\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The AWS generated ID for an export job.\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The user generated name for an export job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\
  \n        },\n        {\n          \"description\": \"The status of a FHIR export job. Possible statuses are SUBMITTED, IN_PROGRESS, COMPLETED, or FAILED.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time an export job was initiated.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time an export job completed.\"\n        }\n      ]\n    },\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS generated ID for the data store from which files are being exported for an export job.\"\n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/OutputDataConfig\"\n        },\n        {\n          \"description\": \"The output data configuration that was supplied when the export job was created.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name used during the initiation of the job.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"An explanation of any errors that may have occurred during the export job.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The properties of a FHIR export job, including the ID, ARN, name, and the status of the job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-export-job-properties-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: ExportJobProperties
---
