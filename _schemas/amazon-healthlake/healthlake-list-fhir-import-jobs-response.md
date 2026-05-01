---
description: ''
layout: schema
name: ListFHIRImportJobsResponse
properties_list:
- description: ''
  name: ImportJobPropertiesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-list-fhir-import-jobs-response-schema.json
slug: healthlake-list-fhir-import-jobs-response
source_filename: healthlake-list-fhir-import-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-import-jobs-response-schema.json\",\n  \"title\": \"ListFHIRImportJobsResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ImportJobPropertiesList\"\n  ],\n  \"properties\": {\n    \"ImportJobPropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImportJobPropertiesList\"\n        },\n        {\n          \"description\": \" The properties of a listed FHIR import jobs, including the ID, ARN, name, and the status of the job. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" A pagination token used to identify the next page of results to return for a ListFHIRImportJobs query. \"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-import-jobs-response-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: ListFHIRImportJobsResponse
---
