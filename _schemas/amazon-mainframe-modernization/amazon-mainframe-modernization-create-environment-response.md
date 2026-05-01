---
description: CreateEnvironmentResponse schema from AWS Mainframe Modernization API
layout: schema
name: CreateEnvironmentResponse
properties_list:
- description: ''
  name: environmentId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-create-environment-response-schema.json
slug: amazon-mainframe-modernization-create-environment-response
source_filename: amazon-mainframe-modernization-create-environment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-environment-response-schema.json\",\n  \"title\": \"CreateEnvironmentResponse\",\n  \"description\": \"CreateEnvironmentResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the runtime environment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-create-environment-response-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: CreateEnvironmentResponse
---
