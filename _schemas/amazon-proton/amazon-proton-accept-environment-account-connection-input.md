---
description: AcceptEnvironmentAccountConnectionInput schema from Amazon Proton API
layout: schema
name: AcceptEnvironmentAccountConnectionInput
properties_list:
- description: ''
  name: id
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-accept-environment-account-connection-input-schema.json
slug: amazon-proton-accept-environment-account-connection-input
source_filename: amazon-proton-accept-environment-account-connection-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-accept-environment-account-connection-input-schema.json\",\n  \"title\": \"AcceptEnvironmentAccountConnectionInput\",\n  \"description\": \"AcceptEnvironmentAccountConnectionInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentAccountConnectionId\"\n        },\n        {\n          \"description\": \"The ID of the environment account connection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-accept-environment-account-connection-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: AcceptEnvironmentAccountConnectionInput
---
