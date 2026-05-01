---
description: ''
layout: schema
name: DescribeFHIRImportJobRequest
properties_list:
- description: ''
  name: DatastoreId
  type: object
- description: ''
  name: JobId
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-describe-fhir-import-job-request-schema.json
slug: healthlake-describe-fhir-import-job-request
source_filename: healthlake-describe-fhir-import-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-import-job-request-schema.json\",\n  \"title\": \"DescribeFHIRImportJobRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastoreId\",\n    \"JobId\"\n  ],\n  \"properties\": {\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS-generated ID of the data store.\"\n        }\n      ]\n    },\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The AWS-generated job ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-import-job-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DescribeFHIRImportJobRequest
---
