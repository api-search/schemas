---
description: ''
layout: schema
name: StartFHIRImportJobResponse
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: DatastoreId
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-start-fhir-import-job-response-schema.json
slug: healthlake-start-fhir-import-job-response
source_filename: healthlake-start-fhir-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-import-job-response-schema.json\",\n  \"title\": \"StartFHIRImportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"JobId\",\n    \"JobStatus\"\n  ],\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The AWS-generated job ID.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The status of an import job.\"\n        }\n      ]\n    },\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS-generated\
  \ data store ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-import-job-response-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: StartFHIRImportJobResponse
---
