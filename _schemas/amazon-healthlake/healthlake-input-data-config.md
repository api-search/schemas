---
description: The input properties for an import job.
layout: schema
name: InputDataConfig
properties_list:
- description: ''
  name: S3Uri
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-input-data-config-schema.json
slug: healthlake-input-data-config
source_filename: healthlake-input-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-input-data-config-schema.json\",\n  \"title\": \"InputDataConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The S3Uri is the user specified S3 location of the FHIR data to be imported into AWS HealthLake. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" The input properties for an import job.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-input-data-config-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: InputDataConfig
---
