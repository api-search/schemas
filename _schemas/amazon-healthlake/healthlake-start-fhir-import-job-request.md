---
description: ''
layout: schema
name: StartFHIRImportJobRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: JobOutputDataConfig
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
schema_file: json-schema/healthlake-start-fhir-import-job-request-schema.json
slug: healthlake-start-fhir-import-job-request
source_filename: healthlake-start-fhir-import-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-import-job-request-schema.json\",\n  \"title\": \"StartFHIRImportJobRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"InputDataConfig\",\n    \"JobOutputDataConfig\",\n    \"DatastoreId\",\n    \"DataAccessRoleArn\",\n    \"ClientToken\"\n  ],\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name of the FHIR Import job in the StartFHIRImport job request.\"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDataConfig\"\n        },\n        {\n          \"description\": \"The input properties of the FHIR Import job in the StartFHIRImport job request.\"\n\
  \        }\n      ]\n    },\n    \"JobOutputDataConfig\": {\n      \"$ref\": \"#/components/schemas/OutputDataConfig\"\n    },\n    \"DatastoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreId\"\n        },\n        {\n          \"description\": \"The AWS-generated data store ID.\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that gives AWS HealthLake access permission.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientTokenString\"\n        },\n        {\n          \"description\": \"Optional user provided token used for ensuring idempotency.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-start-fhir-import-job-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: StartFHIRImportJobRequest
---
