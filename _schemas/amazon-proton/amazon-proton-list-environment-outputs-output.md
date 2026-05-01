---
description: ListEnvironmentOutputsOutput schema from Amazon Proton API
layout: schema
name: ListEnvironmentOutputsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: outputs
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-environment-outputs-output-schema.json
slug: amazon-proton-list-environment-outputs-output
source_filename: amazon-proton-list-environment-outputs-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-outputs-output-schema.json\",\n  \"title\": \"ListEnvironmentOutputsOutput\",\n  \"description\": \"ListEnvironmentOutputsOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyNextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next environment output in the array of environment outputs, after the current requested list of environment outputs.\"\n        }\n      ]\n    },\n    \"outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputsList\"\n        },\n        {\n          \"description\": \"An array of environment outputs with detail data.\"\n  \
  \      }\n      ]\n    }\n  },\n  \"required\": [\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-outputs-output-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListEnvironmentOutputsOutput
---
