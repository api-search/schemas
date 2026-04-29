---
description: ''
layout: schema
name: DescribeFHIRExportJobRequest
properties_list:
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: JobId
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-describe-fhir-export-job-request-schema.json
slug: healthlake-describe-fhir-export-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-export-job-request-schema.json\",\n  \"title\": \"DescribeFHIRExportJobRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\",\n    \"JobId\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS generated ID for the data store from which files are being exported from for an export job.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The AWS generated ID for an export job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-export-job-request-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DescribeFHIRExportJobRequest
---
