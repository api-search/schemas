---
description: ListEnvironmentOutputsInput schema from Amazon Proton API
layout: schema
name: ListEnvironmentOutputsInput
properties_list:
- description: ''
  name: environmentName
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-environment-outputs-input-schema.json
slug: amazon-proton-list-environment-outputs-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-outputs-input-schema.json\",\n  \"title\": \"ListEnvironmentOutputsInput\",\n  \"description\": \"ListEnvironmentOutputsInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The environment name.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyNextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next environment output in the array of environment outputs, after the list of environment outputs that was previously requested.\"\n        }\n \
  \     ]\n    }\n  },\n  \"required\": [\n    \"environmentName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-environment-outputs-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListEnvironmentOutputsInput
---
