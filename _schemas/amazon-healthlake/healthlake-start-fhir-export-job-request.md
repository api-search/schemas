---
description: ''
layout: schema
name: StartFHIRExportJobRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: ClientToken
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-start-fhir-export-job-request-schema.json
slug: healthlake-start-fhir-export-job-request
source_filename: healthlake-start-fhir-export-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-export-job-request-schema.json\",\n  \"title\": \"StartFHIRExportJobRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"OutputDataConfig\",\n    \"DatastoreId\",\n    \"DataAccessRoleArn\",\n    \"ClientToken\"\n  ],\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The user generated name for an export job.\"\n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputDataConfig\"\n        },\n        {\n          \"description\": \"The output data configuration that was supplied when the export job was created.\"\n        }\n      ]\n    },\n    \"DatastoreId\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS generated ID for the data store from which files are being exported for an export job.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name used during the initiation of the job.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientTokenString\"\n        },\n        {\n          \"description\": \"An optional user provided token used for ensuring idempotency.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-export-job-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: StartFHIRExportJobRequest
---
