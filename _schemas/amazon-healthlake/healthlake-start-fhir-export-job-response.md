---
description: ''
layout: schema
name: StartFHIRExportJobResponse
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
schema_file: json-schema/healthlake-start-fhir-export-job-response-schema.json
slug: healthlake-start-fhir-export-job-response
source_filename: healthlake-start-fhir-export-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-export-job-response-schema.json\",\n  \"title\": \"StartFHIRExportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"JobId\",\n    \"JobStatus\"\n  ],\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The AWS generated ID for an export job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The status of a FHIR export job. Possible statuses are SUBMITTED, IN_PROGRESS, COMPLETED, or FAILED.\"\n        }\n      ]\n    },\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\
  \n        },\n        {\n          \"description\": \"The AWS generated ID for the data store from which files are being exported for an export job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-export-job-response-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: StartFHIRExportJobResponse
---
