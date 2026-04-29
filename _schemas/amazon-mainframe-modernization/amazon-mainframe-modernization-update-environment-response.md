---
description: UpdateEnvironmentResponse schema from AWS Mainframe Modernization API
layout: schema
name: UpdateEnvironmentResponse
properties_list:
- description: ''
  name: environmentId
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-update-environment-response-schema.json
slug: amazon-mainframe-modernization-update-environment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-update-environment-response-schema.json\",\n  \"title\": \"UpdateEnvironmentResponse\",\n  \"description\": \"UpdateEnvironmentResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The unique identifier of the runtime environment that was updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-update-environment-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: UpdateEnvironmentResponse
---
