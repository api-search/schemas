---
description: ''
layout: schema
name: DescribeFHIRImportJobResponse
properties_list:
- description: ''
  name: ImportJobProperties
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-describe-fhir-import-job-response-schema.json
slug: healthlake-describe-fhir-import-job-response
source_filename: healthlake-describe-fhir-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-import-job-response-schema.json\",\n  \"title\": \"DescribeFHIRImportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ImportJobProperties\"\n  ],\n  \"properties\": {\n    \"ImportJobProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportJobProperties\"\n        },\n        {\n          \"description\": \"The properties of the Import job request, including the ID, ARN, name, and the status of the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-import-job-response-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DescribeFHIRImportJobResponse
---
