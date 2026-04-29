---
description: ''
layout: schema
name: DescribeFHIRExportJobResponse
properties_list:
- description: ''
  name: ExportJobProperties
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-describe-fhir-export-job-response-schema.json
slug: healthlake-describe-fhir-export-job-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-export-job-response-schema.json\",\n  \"title\": \"DescribeFHIRExportJobResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ExportJobProperties\"\n  ],\n  \"properties\": {\n    \"ExportJobProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExportJobProperties\"\n        },\n        {\n          \"description\": \"Displays the properties of the export job, including the ID, Arn, Name, and the status of the job. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-describe-fhir-export-job-response-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: DescribeFHIRExportJobResponse
---
