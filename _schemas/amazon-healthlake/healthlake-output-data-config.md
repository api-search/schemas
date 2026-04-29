---
description: The output data configuration that was supplied when the export job was created.
layout: schema
name: OutputDataConfig
properties_list:
- description: ''
  name: S3Configuration
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-output-data-config-schema.json
slug: healthlake-output-data-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-output-data-config-schema.json\",\n  \"title\": \"OutputDataConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Configuration\"\n        },\n        {\n          \"description\": \" The output data configuration that was supplied when the export job was created. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"The output data configuration that was supplied when the export job was created.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-output-data-config-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: OutputDataConfig
---
