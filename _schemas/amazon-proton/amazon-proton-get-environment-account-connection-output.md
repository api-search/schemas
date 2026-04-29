---
description: GetEnvironmentAccountConnectionOutput schema from Amazon Proton API
layout: schema
name: GetEnvironmentAccountConnectionOutput
properties_list:
- description: ''
  name: environmentAccountConnection
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-environment-account-connection-output-schema.json
slug: amazon-proton-get-environment-account-connection-output
source_filename: amazon-proton-get-environment-account-connection-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-environment-account-connection-output-schema.json\",\n  \"title\": \"GetEnvironmentAccountConnectionOutput\",\n  \"description\": \"GetEnvironmentAccountConnectionOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentAccountConnection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnection\"\n        },\n        {\n          \"description\": \"The detailed data of the requested environment account connection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environmentAccountConnection\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-environment-account-connection-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetEnvironmentAccountConnectionOutput
---
